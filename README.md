# Extract, Transform and Load - Joining Backers Data

#Overview
Crowdfunding campaigns generally use online platforms to raise the funds for a project by accepting donations from a large number of people. The success of the campaigns are very dependant on how engaged the people are, and how they are contacted. The client for this analysis, asked to have all of their accessible project data moved into a PostgreSQL database. Following the extraction, transformation and loading of their existing spreadsheet data into tables, the client then produced additional data related to project “backers” and asked that it be inserted into a new table in the same database with appropriate relations to the original tables.

# Results
The first step was to extract the "backers" data, into a Pandas DataFrame, and then transform the data. The following image shows the clean Backers DataFrame.

![Backer](https://user-images.githubusercontent.com/46943357/195927505-584dfb89-21b9-4cb5-bcdd-bfcd6963063f.PNG)


After the extraction, we incorporated the data into an existing ERD, to help visualize the Diagram further.

![crowdfunding_db_relationships](https://user-images.githubusercontent.com/46943357/195927849-279a51f7-4b93-4e51-aa12-7813bad60956.png)

Once we have verified that the "backers" information had been correctly incorporated into the database, we had a few more queries run to obtain further information regarding live campaigns that had yet to reach their fundraising objectives and contact information for the existing backers of those campaigns.

![Remaining_Goal](https://user-images.githubusercontent.com/46943357/195928489-ad087947-7850-4137-ae66-06891b54fcca.PNG)

# Summary
Through the process known as ETL (Extract, Transform, Load) We are able to create databases that, when combined with appropriate queries, are capable of providing required information in an efficient and elegant manner.
