# COP4331 COLORS Project

## What is this?
This is a basic LAMP stack web app built for my COP4331 lab. It's a simple dashboard where users can log in and add/search Colors. 

## Tech Stack
- **Frontend:** HTML, CSS, Vanilla JS
- **Backend:** PHP 
- **Database:** MySQL
- **Server:** Ubuntu 

## Setup Instructions
To host this yourself, you'll need a Linux server with Apache, MySQL, and PHP already installed.
1. Clone this repo to your server.
2. Copy everything inside the `public/` folder directly into your web root (usually `/var/www/html/`).
3. Copy the `api/` folder into your web root and rename it to `LAMPAPI` (so the path becomes `/var/www/html/LAMPAPI/`).
4. Open the PHP files in the API folder and swap out the generic database connection strings with your actual MySQL username and password.

## Running the App
1. Build your database by creating the `Users` and `Colors` tables in MySQL.
2. Make sure your Apache server is running.
3. Open a browser and go to your server's IP address or domain name. 
4. Log in with a valid account to test the color dashboard.

## Notes & Limitations
- Passwords are hashed on the frontend using MD5 before being sent to the database.
- The PHP backend assumes the database is hosted on the exact same server (`localhost`).