# Text Similarity and Merge Tool

This Java-based project aims to identify similarities between sentences extracted from books or different written texts and merge them based on identified similarities. The merged texts are then displayed on a web interface. The backend of the project utilizes Spring Framework for handling business logic and integrating it with the frontend, which is developed using HTML.

## Overview

The project uses Spring Framework, a powerful open-source application development framework for Java, to merge the backend and frontend components seamlessly. The frontend interface is designed using HTML, allowing users to input and merge multiple texts, which are then processed by Java backend services.

MongoDB, a NoSQL database, is used as the data storage solution for this project.

## Features

- **Text Merge Functionality**:
  - Users can input multiple texts through an HTML page.
  - Java backend processes and merges the texts based on similarities.
  - Merged texts are stored in MongoDB.

- **Web Interface**:
  - HTML-based web interface for user interaction.
  - Allows dynamic input of texts and merging operations.
  - Displays the merged text and the time taken for merging on the web page.

## Methodology

### Components and Classes

- **MergedTextController**:
  - Handles HTTP requests and calls methods from `MergedTextService`.
  - Detects user interactions on the web page and invokes appropriate methods.

- **MergedTextService**:
  - Performs text merging and processing operations.
  - Manages the business logic for merging texts based on similarities.

- **MergedTextRepository**:
  - Extends `MongoRepository` interface to handle database operations.
  - Provides methods to store merged texts in MongoDB.

- **MergedTextDto**:
  - Data transfer object that facilitates passing data between frontend (HTML) and backend (Java).
  - Enables dynamic handling of text inputs by representing them as lists.

