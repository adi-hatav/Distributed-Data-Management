# Distributed-Data-Management

The following project was created by Adi Hatav and Tamar Dufour Dror, as part of the "Distributed Data Management" course at the Technion. 

Since we dealt with very large datasets of a cable - company, we utilized a virtual machine (Azure Databricks) and PySpark. Sample datasets can be found in the attached zip file.

The project consists of two main parts:
Part 1:

A.	Spam Detection – In this section, we deleted records that met several cumulative conditions defined as spam.

B.	Fragmentation – First, we ranked the records according to the level of popularity in each DMA. Afterward, we found the "wealth score" for each DMA, and then we found its 8 most popular genres (with a limitation: a genre can’t be duplicated).
Finally, we divided the data to directories, each one containing a fragment based on DMA + genre.

Part 2:

A.	Static Data Analysis – In this section we selected recommended records for the customers, according to their demographic profile.
First, we explored and analyzed the "demographic data". Then, we used PCA to estimate the number of clusters in our data. Accordingly, we ran KMeans algorithm, and divided the households to clusters.
Then, we found the popularity - rating of each record in every cluster.

B.	Dynamic Data Analysis, Streaming – In this section, we used PySpark Streaming to extract "viewing data" from Kafka. While streaming, we repeated the analysis task, for each trigger’s data.
