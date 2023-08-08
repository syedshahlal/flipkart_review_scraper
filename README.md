# Web Scraping Flipkart Product Reviews
<img src="https://logos-world.net/wp-content/uploads/2020/11/Flipkart-Emblem.png" width="80" height="40" alt="Flipkart Logo">

In this project, I developed a web scraping application using Flask, which allows users to fetch product reviews, ratings, comments, and commenter names from the Flipkart website. The scraped data is displayed through a simple user interface built using HTML.

## Project Overview

### Technologies Used
- Flask: A Python web framework used for creating the backend of the application.
- BeautifulSoup: A Python library used for parsing HTML and XML documents to extract data.
- Requests: A Python library used for making HTTP requests to fetch web pages.
- HTML: Used for building the user interface.

### Project Structure
The project is organized into the following main files and directories:

1. `app.py`: This is the main Python file that defines the Flask application. It contains routes to handle user requests and initiate web scraping.

2. `templates/`: This directory contains the HTML templates for the user interface.

3. `static/`: This directory contains static files such as CSS, JavaScript, and images (if any) used in the user interface.

4. `scraper.py`: This Python file contains the functions for web scraping Flipkart product reviews. It uses BeautifulSoup and Requests libraries to extract relevant data.

## Web Scraping Process

### 1. User Input
The user is required to input the URL of the Flipkart product page they want to scrape. They can enter the URL into a text input field on the user interface.

### 2. Fetching HTML
When the user submits the URL, the Flask backend receives the URL and makes an HTTP request to the Flipkart website to fetch the product page's HTML content.

### 3. Parsing HTML
The received HTML content is then passed to the BeautifulSoup library, which parses the HTML and extracts the necessary information like review ratings, comments, and reviewer names.

### 4. Data Display
The extracted data is then displayed on the user interface, presenting the user with product reviews, ratings, comments, and commenter names.

## Deployment

The application is deployed as a simple HTML web application. The Flask backend is hosted on a server, and the HTML templates are served to users who access the application through their web browsers.

## Usage

1. Clone the repository to your local machine.
2. Install the required Python libraries using `pip install flask beautifulsoup4 requests`.
3. Run the Flask application using `python app.py`.
4. Access the application in your web browser by visiting `http://localhost:5000` or the appropriate server URL.

### Note:
- Web scraping may be subject to terms of service or legality on some websites. Ensure that you are allowed to scrape data from the Flipkart website before using the application.

## Future Enhancements

- Implementing pagination support to scrape multiple pages of reviews.
- Adding data filtering and sorting options on the user interface.
- Improving the user interface with more interactive features.

---

With this project, users can easily extract and view product reviews from the Flipkart website, making it a useful tool for gathering insights into customer opinions and sentiments. Remember to comply with web scraping policies and avoid any misuse of the scraped data. Happy scraping!
