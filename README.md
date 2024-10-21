# Implementation for Data Engineering module
Real-time data backend for tracking football player locations based on video footage

This project aims to simulate a simplified real-time data backend for tracking football player locations, enabling analyses such as formation changes over time. Using the SoccerTrack dataset from Kaggle (https://www.kaggle.com/datasets/atomscott/soccertrack) , which annotates football game footage with player coordinates, the data will first be streamed into Kafka as raw four-column bounding boxes. A Kafka Streams application will then transform these into simpler two-column x-y coordinates, making them easier to visualize. The transformed coordinates will be stored in MongoDB for further analysis.
