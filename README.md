
Django REST API – Basic CRUD

This is a simple REST API built using Django and Django REST Framework (DRF). It demonstrates how to build RESTful endpoints for basic CRUD operations using a model
in a modular and beginner-friendly format.

---

Features

Django & Django REST Framework setup
CRUD endpoints for managing a model
SQLite database (default)
Clean and modular code structure
Easily extendable (authentication, filtering, pagination, etc.)

---

Installation (Windows – CMD)

 1. Clone the repository

cmd
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name\Django\newproject


 2. Set up a virtual environment

cmd
python -m venv env
env\Scripts\activate


3. Install required packages

cmd
pip install -r requirements.txt


> If `requirements.txt` is missing, manually install:

cmd
pip install django djangorestframework


4. Run migrations

cmd
python manage.py migrate


5. Start the development server

cmd
python manage.py runserver


---

 API Endpoints
These are the RESTful API endpoints available for the User model:

Method	 Endpoint	            Description
GET	     /api/users/	        List all users
POST	   /api/users/	        Create a new user
GET	     /api/users/<id>/	    Retrieve user by ID
PUT	     /api/users/<id>/	    Update user by ID
DELETE	/api/users/<id>/	    Delete user by ID

---

 Project Structure
 
 bash
Django/
├── .git/
├── .vscode/
├── env/                      # Python virtual environment
└── newproject/
    ├── api/                  # Django app
    │   ├── admin.py
    │   ├── apps.py
    │   ├── models.py
    │   ├── views.py
    │   ├── urls.py
    │   ├── serializer.py
    │   └── migrations/
    ├── newproject/           # Project settings
    │   ├── __init__.py
    │   ├── settings.py
    │   ├── urls.py
    │   └── wsgi.py
    ├── db.sqlite3
    └── manage.py


---

What's Next (Coming Soon)
Token-based authentication
Filtering and pagination
Swagger/OpenAPI documentation
Docker support

---

Learning Goals

This project helped me:

 Understand Django REST Framework fundamentals
 Build and connect serializers, views, and URLs
 Handle database models and migrations
 Prepare for larger backend projects

---

License

This project is open source and available under the [MIT License](LICENSE).

---

Questions or Suggestions?

Feel free to open an issue or submit a pull request if you have ideas or find bugs!


