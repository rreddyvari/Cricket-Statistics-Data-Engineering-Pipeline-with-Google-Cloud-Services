# Building a Cricket Statistics Data Engineering Pipeline with Google Cloud Services

In data engineering, transforming data collection into insightful visualizations is a journey full of challenges and achievements. This guide outlines building a cricket statistics pipeline with Google Cloud services, from fetching data with the Cricbuzz API to creating a Looker Studio dashboard, ensuring a smooth data analysis and visualization process.

### Architecture

![Architecture](https://github.com/mohitrpatil/Cricket-statistics-data-engineering-GCP/blob/main/Architecture.png)

### Integrating Python with the Cricbuzz API for Data Collection
Our project kicks off by leveraging Python's capability to interact with APIs. We will explore how to extract cricket statistics using the Cricbuzz API, utilizing Python to efficiently fetch the necessary data.

### Securing Data in Google Cloud Storage (GCS)
Once the data is obtained, our next step involves preserving it securely in the cloud. We’ll explore how to store this data in a CSV format within Google Cloud Storage (GCS), ensuring accessibility and scalability for future processing.

### Setting Up a Cloud Function Trigger
Following data storage, we move on to establishing a Cloud Function. This function is designed to activate upon new file uploads to our GCS bucket, marking the starting point for the upcoming stages of our data processing workflow.

### Activating the Cloud Function
The Cloud Function is programmed with detailed code to accurately launch a Dataflow job. We will focus on managing triggers and forwarding the necessary parameters to start the Dataflow job effortlessly, facilitating an uninterrupted data processing sequence.

### Implementing a Dataflow Job for Data Transfer to BigQuery
At the heart of our workflow is the Dataflow job, initiated by the Cloud Function. This job is responsible for moving data from the GCS CSV file to BigQuery. We will fine-tune the job configurations to maximize efficiency and ensure precise data transfer into BigQuery.

### Developing a Looker Dashboard
Lastly, we will delve into utilizing BigQuery as a datasource for Looker Studio. By setting up Looker to link with BigQuery, we aim to construct an engaging dashboard. This dashboard will act as the center for visualization, offering deep insights through the analysis of our cricket statistics data.
![Looker](https://github.com/mohitrpatil/Cricket-statistics-data-engineering-GCP/blob/main/Looker.png)
