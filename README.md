## Recepi API using Django
1. Docker file
2. Docker ignore

    Run \recepi-api>docker build .

3. Add docker-compose.yml file --> recepi-api>docker-compose build
4. recepi-api>docker-compose run --rm app sh -c "flake8"
5. Create Django project:\recepi-api>docker-compose run --rm app sh -c "django-admin startproject app ."
6. Run the project: \recepi-api>docker-compose up

7. Running the test project:\recepi-api>docker-compose run --rm app sh -c "python manage.py test"
8. Creating new core project: docker-compose run --rm app sh -c "python manage.py startapp core"
9. Checking linting: docker-compose run --rm app sh -c "python manage.py wait_for_db && flake8"
10. Migration: docker-compose run --rm app sh -c "python manage.py makemigrations"
               docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"

11. Creating super user: docker-compose run --rm app sh -c "python manage.py createsuperuser"