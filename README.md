# 🛒 Mini E-commerce REST API

A simple E-commerce REST API built with **Django REST Framework**.

## 🚀 Features

- Category CRUD
- Product CRUD
- Product Filtering (by category, price)
- Product Searching (by name)
- Product Ordering (by price, created_at)
- Pagination
- Token Authentication
- Order API with stock validation

## 🛠️ Tech Stack

- Django
- Django REST Framework
- django-filter
- SQLite
- Token Authentication

## ⚙️ Setup

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

## 🔗 API Endpoints

### Auth
- `POST /api/auth/register/`
- `POST /api/auth/login/`
- `POST /api/auth/logout/`

### Category
- `GET /api/categories/`
- `POST /api/categories/`
- `GET /api/categories/{id}/`
- `PUT /api/categories/{id}/`
- `DELETE /api/categories/{id}/`

### Product
- `GET /api/products/`
- `POST /api/products/`
- `GET /api/products/{id}/`
- `PUT /api/products/{id}/`
- `DELETE /api/products/{id}/`

**Query Params:**
- `?search=phone`
- `?category=1`
- `?ordering=price`
- `?page=2`

### Order
- `GET /api/orders/`
- `POST /api/orders/`
- `POST /api/orders/`

## 🔐 Authentication

Token-based. Login করে token নিন, তারপর header-এ পাঠান:

```
Authorization: Token <your_token>
```

## 👨‍💻 Author

Redwan Ahmed Utsob
