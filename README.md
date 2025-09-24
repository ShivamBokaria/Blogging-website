# Django Blog Website

This is a Django-based website that allows users to post, delete, and update blogs. Users can also maintain their profiles on the website. The project includes a registration system where users can create an account, login, and reset their password through email.

## Features

- User Registration: Users can create an account by providing their details such as username, email, and password.

- Login and Authentication: Registered users can log in to the website using their credentials. Authentication is implemented to ensure secure access to user-specific features.

- Blog Creation: Users can create blog posts by providing a title, content, and optionally uploading an image.

- Blog Editing and Deletion: Users have the ability to edit or delete their own blog posts.

- Profile Management: Each user has a profile page where they can update their personal information, including their profile picture.

- Password Reset: If a user forgets their password, they can initiate a password reset process. An email will be sent to their registered email address containing a unique link. By following the link, the user can reset their password.

## Installation

1. Clone the repository:

```
git clone https://github.com/your-username/django-blog-website.git
```

## Setup and Usage

To set up and run the Django Blog Website project, follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command in the project directory:
   ```
   pip install -r requirements.txt
   ```

3. Set up the database by running the necessary migrations. Use the following commands:
   ```
   python manage.py makemigrations
   python manage.py migrate
   ```

4. Create a superuser account to access the admin interface and manage the website. Run the following command and follow the prompts:
   ```
   python manage.py createsuperuser
   ```

5. Start the development server by running:
   ```
   python manage.py runserver
   ```

6. Open a web browser and navigate to `http://localhost:8000` to access the Django Blog Website.

7. Use the admin interface at `http://localhost:8000/admin` to manage articles, user accounts, comments, and other website functionalities.

## Configuration

- Email Settings: Configure the email settings in the `settings.py` file to enable the password reset functionality. You will need to provide your email service provider's SMTP details, such as the host, port, username, and password.

- Secret Key: Generate a new secret key and update the `settings.py` file with the new value. It is recommended to keep the secret key confidential and not share it publicly.

## Usage

- Create an account by clicking on the "Register" link on the homepage and providing the necessary information.

- Log in using your credentials to access the blog creation, editing, and deletion features.

- Manage your profile by navigating to the profile page and updating your information.

- In case you forget your password, click on the "Forgot Password" link on the login page and follow the instructions in the email to reset it.

