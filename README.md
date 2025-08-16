# Online Bookstore — Django + PostgreSQL
Full‑stack e‑commerce demo with **auth**, **product listing & search**, **session cart**, and **orders**.

## Quickstart
```bash
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Mac/Linux

pip install -r requirements.txt

python manage.py migrate
python manage.py createsuperuser
python manage.py seed_data   # add sample categories + products
python manage.py runserver
```
Open: http://127.0.0.1:8000/

## Features
- Authentication (signup/login/logout)
- Product catalog (categories, pagination, search `?q=`)
- Product detail page
- Session‑based cart (add/remove/total)
- Checkout → Order & OrderItems
- Bootstrap UI

## Notes
- Dev DB: SQLite. For production, configure PostgreSQL and set env vars, then update `DATABASES` in `bookstore/settings.py`.
- Static files: WhiteNoise for prod.
- Images: optional via `Product.image`.
