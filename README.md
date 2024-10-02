# Flask Large-Scale Application Template

🎉 **Welcome to the Flask Large-Scale Application Template!** 

This is an application template designed for large Flask applications with integrated Flask-SQLAlchemy. It helps to organize your project in a scalable and maintainable structure.

## Project Structure 📂
```plaintext
.
├── app
│   ├── extensions.py
│   ├── __init__.py
│   ├── main
│   │   ├── __init__.py
│   │   └── routes.py
│   ├── models
│   │   ├── post.py
│   │   └── question.py
│   ├── posts
│   │   ├── __init__.py
│   │   └── routes.py
│   ├── questions
│   │   ├── __init__.py
│   │   └── routes.py
│   └── templates
│       ├── base.html
│       ├── index.html
│       ├── posts
│       │   ├── categories.html
│       │   └── index.html
│       └── questions
│           └── index.html
├── config.py
```

## Getting Started 🚀

### Prerequisites
- Python 3.8+
- pip (Python package installer)

### Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/loyal812/flask-template.git
    cd flask-template
    ```

2. **Create a virtual environment:**
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

4. **Set up Environment Variables:**
   Create a `.env` file based on the `.env.example` and configure the necessary settings such as database URL and secret keys.

### Configuration 🛠️

All configurations are done in the `config.py` file. Adjust the configurations based on the environment (development, testing, production).

### Database Setup
1. **Initialize the Database:**
    ```sh
    flask db init
    ```

2. **Generate Migration:**
    ```sh
    flask db migrate -m "Initial migration."
    ```

3. **Apply Migrations:**
    ```sh
    flask db upgrade
    ```

### Running the Application

```sh
flask run
```

This will start the server locally at http://127.0.0.1:5000/.

## Structure Explanation 📘
- **app/extensions.py**: For initializing and configuring Flask extensions.
- **app/main/routes.py**: Main application routes.
- **app/models/post.py**: Database models related to posts.
- **app/models/question.py**: Database models related to questions.
- **app/posts/routes.py**: Routes related to posts functionality.
- **app/questions/routes.py**: Routes related to questions functionality.
- **app/templates**: Directory for HTML templates. Organized into subdirectories for different modules.

## Contributing 🤝

Please read the [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests to us.
