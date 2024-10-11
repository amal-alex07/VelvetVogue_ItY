# E-Commerce Backend

This is the backend component of an e-commerce website built with Django. It provides APIs for user authentication, product management, shopping cart functionality, and order processing.

## Features

- User registration and authentication
- Product listing and management
- Shopping cart functionality
- Order management
- Payment integration with Stripe

## Technologies Used

- **Backend**: Python, Django, Django REST Framework
- **Database**: PostgreSQL (or SQLite for development)
- **Payment Gateway**: Stripe
- **Environment**: Virtualenv

## Getting Started

### Prerequisites

- Python 3.x
- PostgreSQL (if using PostgreSQL as the database)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/ecommerce_backend.git
   cd ecommerce_backend


### Set up the virtual environment

python -m venv venv
source venv/bin/activate  # On Windows use venv\Scripts\activate



### Install the required dependencies:

pip install django djangorestframework django-cors-headers psycopg2  # For PostgreSQL


### Configure the database:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'your_db_name',
        'USER': 'your_db_user',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}


### Create a new Django project and app:

#### Create a new Django project

django-admin startproject ecommerce_project .

#### Create a new app for managing products and orders

python manage.py startapp shop

### Run migrations:

python manage.py migrate

### Run the development server:

python manage.py runserver

## API Endpoints

#### POST /api/register/ - Register a new user
#### POST /api/login/ - User login
#### GET /api/products/ - List all products
#### GET /api/products/{id}/ - Get product by ID
#### POST /api/cart/ - Create a new cart
#### POST /api/orders/ - Create a new order

### Contributing
Feel free to contribute to this project. Fork the repository, create a feature branch, and submit a pull request.