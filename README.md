# Harrison's Developer Blog

I created a personal developer blog using Flask, Jinja, and Bootstrap. This website is a refactor of a bootstrap template in order to run on a Flask Webapp. The point of the blog would be to post articles about my career progression and projects as a software developer. I've created a few sample posts and comments to demonstrate the would-be functionality of the website.

Articles, users, and comments are stored on a local sqlite database, and retreived using Flask-SQLAlchemy.

I used gunicorn to deploy the webapp to Heroku for testing, but the app is currently not deployed to a live server.

📚 **Tech Stack**:
- HTML, Jinja
- CSS, Bootstrap
- Flask
- Sqlite / SQLAlchemy

🧰 **Full CRUD operation**:
1. Create blog posts & comments 
2. View all blog posts & comments
3. Update/Edit blog posts & comments
4. Delete blog post & comments

🔐 **User Sessions & Auth with Flask**:
- Login and Logout
- Recognize administrator user
- Protect routes from unauthorized users
- View blog posts and post comments by user

___

## How to Run the Webapp Locally:

### Installation and Setup

1. Clone the repository, and navigate to the webapp's directory:
    ```bash
    git clone <project_url>
    
    cd <project_directory>

    cd /Harrisons-Blog
    ```

2. Install the package requirements:
    ```
    pip install -r requirements.txt
    ```

3. Run the webapp:
    ```
    python3 server.py
    ```

### Admin Login

1. Using the site header, navigate to the `Login` page.

2. Login with the following credentials:
    ```
    username: admin
    password: testpass
    ```

3. You now have the ability to create, edit, and delete blog posts.

### User Login:

1. Using the site header, navigate to the `Login` page.

2. Login with the following credentials:
    ```
    username: user2
    password: testpass
    ```

3. You can now view the site of a regular user without admin privelages.
    - You can post comments
    - You can view posts, even when logged out.

___

## Website Demo:

![Website Demo](./demo.gif)