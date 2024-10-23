# Tweet Application - Django Project

## Overview
This is a simple Django-based Twitter-like application where users can create, view, and delete tweets. It leverages Django's ORM for database management and built-in authentication for user registration and login functionality.

## Features
- **User Authentication**: Users can register, log in, and log out using Django's built-in authentication system.
- **Create Tweet**: Logged-in users can create and post new tweets. The form for creating tweets is simple and user-friendly.
- **List of Tweets**: The home page shows all tweets from users in chronological order, with pagination if necessary.
- **Edit/Delete Tweets**: Users can edit or delete their own tweets via the tweet management interface.
- **Responsive Design**: The application is designed to be accessible on different screen sizes, providing a mobile-friendly user experience.
- **Admin Interface**: Admins can manage users and tweets through Django’s built-in admin interface.
  
## Screenshots

### Home Page - Tweet List
<img width="947" alt="image" src="https://github.com/user-attachments/assets/22d14569-d81f-4350-a2a6-b4b8d7dc1fb0">

### Create Tweet Page
<img width="950" alt="image" src="https://github.com/user-attachments/assets/27653147-c795-4345-b5ca-e1b3e9602581">

### Registration Page
<img width="953" alt="image" src="https://github.com/user-attachments/assets/3dee2b90-fc88-4f21-8c94-da40e95b26a4">

### Login Page
<img width="959" alt="image" src="https://github.com/user-attachments/assets/d4eb6a58-d505-4bc9-ab7d-ef556d5ecc3f">

### Logged in page
<img width="946" alt="image" src="https://github.com/user-attachments/assets/bb2e5534-2a23-4426-b678-d8f4bced0031">

### Deletion confirmation page
<img width="957" alt="image" src="https://github.com/user-attachments/assets/ac95ce20-678b-409c-b459-5efc70dd3161">



## Project Structure

```bash
mysite/
├── db.sqlite3               # SQLite database
├── manage.py                # Django management script
├── mysite/
│   ├── settings.py          # Project settings
│   ├── urls.py              # Global URL configuration
│   └── ...                  # Other Django configurations
│
├── tweet/
│   ├── migrations/          # Database migrations
│   ├── templates/           # HTML templates for tweets and layout
│   │   ├── index.html       # Home page for displaying tweets
│   │   ├── tweet_form.html  # Form for creating tweets
│   │   ├── tweet_confirm_delete.html  # Confirmation page for deleting tweets
│   └── ...
│   ├── admin.py             # Admin configuration
│   ├── models.py            # Data models for the Tweet app
│   ├── forms.py             # Forms for creating and deleting tweets
│   ├── urls.py              # URL routing for tweet-related views
│   ├── views.py             # Views to handle tweet logic
│   └── ...


## Prerequisites

- Python 3.x
- Django (installed via pip)
- SQLite (default database)

## Setup Instructions

1. **Clone the repository**:
    ```
    git clone <repository-url>
    cd mysite
    ```

2. **Install dependencies**:
    Create a virtual environment and install Django:
    ```
    python3 -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    pip install django
    ```

3. **Run migrations**:
    Apply migrations to set up the database schema:
    ```
    python manage.py migrate
    ```

4. **Run the development server**:
    Start the Django development server:
    ```
    python manage.py runserver
    ```

5. **Access the application**:
    Open your web browser and go to `http://127.0.0.1:8000/` to see the tweet application.

## How to Use

- **Register**: Create an account through the registration page.
- **Log in**: Use your credentials to log in.
- **Create Tweet**: Go to the tweet creation page and post a tweet.
- **View Tweets**: Access the homepage to view all posted tweets.
- **Delete Tweets**: Click on the delete button to remove a tweet you posted.

## Project Files of Interest

- **`models.py`**: Defines the Tweet model.
- **`forms.py`**: Includes the form used to submit new tweets.
- **`views.py`**: Handles the logic for creating, listing, and deleting tweets.
- **`urls.py`**: Maps URLs to corresponding views.
- **Templates**:
    - `index.html`: Home page displaying the tweet list.
    - `tweet_form.html`: Form for creating tweets.
    - `tweet_confirm_delete.html`: Confirmation page for deleting tweets.


