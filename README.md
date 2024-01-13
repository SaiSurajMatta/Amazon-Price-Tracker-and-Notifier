# Amazon Price Tracker and Notifier

## Overview

This Python script allows you to track the price of a specific product on Amazon and receive email notifications when the price drops below a certain threshold. The project utilizes web scraping techniques to extract product details, and it is designed to run at scheduled intervals to keep you updated on price changes.

## Features

- **Web Scraping:** Utilizes BeautifulSoup library to scrape product details (title and price) from Amazon.
- **Data Logging:** Stores product information in a CSV file with timestamps to track price changes over time.
- **Email Notification:** Sends email notifications using the smtplib library when the price falls below a predefined value.
- **Automation:** Runs the price-checking process at scheduled intervals using a while loop and time.sleep.

## How to Use

1. Clone the repository:

```bash
git clone https://github.com/SaiSurajMatta/Amazon-Price-Tracker-and-Notifier
```

2. Install the required libraries:

```bash
pip install beautifulsoup4 requests pandas
```

3. Update the script with your Amazon product URL and Gmail credentials for email notifications.

4. Run the script:

5. Customize the price threshold and email message as needed.

## Configuration

- **URL:** Replace the `URL` variable with the Amazon product URL you want to track.
- **Email Credentials:** Update the email credentials in the `send_mail` function with your Gmail address and password.

## Scheduled Execution

The script is set to run indefinitely with a 24-hour interval between price checks. You can adjust the interval by modifying the `time.sleep` duration.

## Dependencies

- BeautifulSoup
- Requests
- Pandas

Feel free to customize the readme to better suit your project and provide more details about its purpose and structure.
