
This project focuses on creating a web-based application using Flask to collect participants' data related to their income and spending. The data is saved in MongoDB, processed using Python, and visualized with Pandas and Matplotlib in a Jupyter notebook. The objective is to analyze spending patterns ahead of a healthcare product launch, with the application hosted on AWS EC2.

Key Features
Data Collection: Users can enter their age, gender, total income, and expenses across categories such as utilities, entertainment, school fees, shopping, and healthcare.
Data Storage: All user information is stored in MongoDB for future analysis.
Data Processing: Python scripts process the collected data, store it in CSV format, and create visualizations to aid in analysis.
Deployment: The Flask application is deployed on AWS EC2 for easy remote access.
Prerequisites
Python 3.x
Flask framework
pymongo for MongoDB integration
pandas
matplotlib
seaborn
Installation and Configuration
1. Launch AWS EC2 Instance
Start an EC2 instance with either Amazon Linux or Ubuntu, and connect to it using SSH.

2. Install Required Packages
First, update the package manager and install the necessary software, including Python, pip, and relevant libraries such as Flask, MongoDB drivers, and data analysis tools.

3. MongoDB Setup
Install MongoDB on your EC2 instance, if not already available, and configure it to run as a background service.

4. Clone the Project Repository
Clone the repository containing the project files to your EC2 instance and navigate into the project directory.

5. Modify Flask Configuration
Update the connection settings in the Flask application to point to your MongoDB instance.

6. Running the Flask Application
Start the Flask web application, which will be accessible through your EC2 instance's public IP.

How to Use
Users can input their details, including age, gender, income, and categorized expenses, via the web form.
Submitting the form stores the information in MongoDB for future processing.
You can then analyze and visualize the data using the provided Python scripts and Jupyter notebook.
Project File Structure
app.py: The Flask application file responsible for running the web app.
data_processing.py: Python script to process user data and generate a CSV file.
requirements.txt: A list of dependencies required to run the project.
templates/: HTML templates used for rendering web pages.
static/: Contains static files such as CSS and JavaScript.
user_data.csv: A CSV file where the processed user data is stored.
analysis.ipynb: Jupyter notebook used for data analysis and visualization.
README.md: This readme file containing project information.
