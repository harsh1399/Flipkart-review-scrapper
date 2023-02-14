# Flipkart-review-scrapper

A web application that collects reviews of the products from Flipkart E-Commerce Website. Developed using Flask framework, the application caches the reviews into a cloud database (MongoDB Atlas) to improve the performance of the application. The application uses the Request library to send HTTP requests and uses BeautifulSoup to parse the response.

### Architechture
The application uses client server architechture. The client sends a request to get the reviews of a particular product, subsequently, the server first checks the database for the product review. If the database doesn't contain any info about the product the server sends a HTTP request to collect the required info.

### Repo Structure
 - Static - It contains all the CSS files.
 - Templates - Contains all the HTML files for the web app.
 - new_app.py - Python file for flask application
 - requirements.txt - contains all the necessary libraries
 
### How to run the app - 

1. Clone the repository using the following command - 
```
git clone https://github.com/harsh1399/Flipkart-review-scrapper.git
```

2. Create a virtual environment and install the required libraries -
```
pip install -r requirements.txt
```

3. To run the flask app - 
```
flask --app new_app run
```
