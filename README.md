## Recepi API using Django
1. Docker file
2. Docker ignore
    
    Run \recepi-api>docker build .

3. Add docker-compose.yml file --> recepi-api>docker-compose build
4. recepi-api>docker-compose run --rm app sh -c "flake8"
5. Create Django project:\recepi-api>docker-compose run --rm app sh -c "django-admin startproject app ."