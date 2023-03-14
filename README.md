### **Airbnb dbt project!**

About Data:
The data is from the inside Airbnb's data sharing website. It is Airbnb listings about Berlin, Germany.

![image](https://user-images.githubusercontent.com/46944817/223885700-d7304afe-2735-4214-b381-2d548dfd3273.png)


### **Tech Stack and Data Pipeline:**

Source file is Cloud storage, ingested into managed datawarehouse Snowflake(Bigquery, Redshift can also be used) . dbt sits on top of Snowflake for transformation and transformed data is used by visualization layer.

<img width="1080" alt="Drawing (1)" src="https://user-images.githubusercontent.com/46944817/223884321-46366fdb-446b-4694-a448-1e34aa4f3d32.png">




### **Below is the DAG for processing.**

![dbt-dag](https://user-images.githubusercontent.com/46944817/223878666-38417ece-4215-47f0-bf5d-5275bc43b71b.png)

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices

### Creating a Virtual env for mac m1 users (homebrew)-

### List all versions of python installed:

brew list | grep python

### create an env using below:

virtualenv --python=/opt/homebrew/bin/python3.9 venv
