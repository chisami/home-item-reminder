# home-item-reminder
The Item Reminder application records product names, expiry dates, and other relevant information in Google Sheets via a Telegram bot and Google Apps Script. It sends reminders to users through Telegram before items expire.

# Item Reminder Application

## Overview
The **Item Reminder Application** is a powerful tool designed to help users keep track of product expiry dates. By leveraging Telegram bots, Google Sheets, and image recognition technology, this application allows users to create, update, view, and delete item reminders efficiently. Users receive timely notifications before items expire, ensuring they never miss important dates.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features
- **Telegram Integration**: Two bots to handle item reminders and image processing.
  - **Item-Reminder Bot**: Manages CRUD operations for item records.
  - **Expiry Date Bot**: Allows users to create reminders by scanning product photos.
  
- **Google Sheets Database**: Stores product information including names, expiry dates, and other relevant details.

- **Image Uploads**: Users can upload product images that are processed to extract relevant information.

- **Web Management Interface**: A user-friendly web page built with Google Apps Script for managing item records.

- **Automated Reminders**: Scheduled checks for item expiry with notifications sent via Telegram.

## Technologies Used
- **Telegram Bots**: For user interaction and notifications.
- **Google Apps Script**: For backend logic and integration with Google Sheets.
- **Python**: For image processing and API interactions.
- **Google Sheets**: To store product data.
- **Google Drive API**: To upload and manage product images.

## Getting Started

### Prerequisites
1. A Telegram account to interact with the bots.
2. A Google account to access Google Sheets and Google Drive.
3. Basic knowledge of Python and JavaScript (Google Apps Script).

### Installation
1. **Create Telegram Bots**:
   - Use [BotFather](https://core.telegram.org/bots/api) on Telegram to create two bots:
     - `@item_reminder_bot` (for managing reminders)
     - `@expiry_date_bot` (for scanning product images)
   - Save the access tokens provided by BotFather.

2. **Set Up Google Sheets**:
   - Create a new Google Sheet to store product information.
   - Note the Sheet ID from the URL for later use.

3. **Deploy Google Apps Script**:
   - Open Google Apps Script and create a new project.
   - Implement the backend logic for the Item-Reminder Bot and the web management interface using the provided code snippets.

4. **Set Up Python Environment**:
   - Install necessary libraries:
     ```
     pip install Flask google-api-python-client Pillow
     ```
   - Write the Python script for the Expiry Date Bot that handles image uploads and uses an API for image recognition.

5. **Configure Google Drive API**:
   - Enable the Google Drive API in your Google Cloud Console.
   - Create credentials and download the JSON file for authentication.

## Usage
1. Start interacting with the `@item_reminder_bot` to add, update, view, or delete item reminders by sending text commands.
2. Use `@expiry_date_bot` to upload product images directly from your device. The bot will extract relevant information using an API call.
3. Access the web management interface to view and manage all stored items conveniently.

### Scheduling Reminders
The Item-Reminder Bot will automatically check for items nearing their expiry dates based on a predefined schedule set in your Google Apps Script. Users will receive notifications through Telegram before an item expires.



---

Thank you for using the Item Reminder Application! We hope it helps you manage your products effectively!
