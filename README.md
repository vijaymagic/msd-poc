# msd-platform-interview-challenge

## Description

Your mission, should you choose to accept it, is to containerise an application
we have created for you and host it in AWS with a TLS endpoint.

Specifically, you need to:

- Add a Dockerfile for the application in `src/`
- Describe a plan to create a AWS infrastructure which
   - Runs the container workload (ECS / K8 / Ec2 / Or anything)
   - Exposes the application to the internet over HTTPS in some way
- Automate the same. 

Please be mindful of AWS costs! We don't want you to run up a bill. It is
possible with free-tier resources but you may use some low cost resources if
you wish.

## Application

The application is a Python mock REST API for emails. It uses
[poetry](https://python-poetry.org/docs/) for dependency management. In case
you're not familiar, poetry takes care of python virtualenvs to avoid dependency
conflicts, and it locks the dependency tree with `poetry.lock` to provide
repeatable builds. The app should have it's dependencies installed with `poetry
install` run from the `src/` folder.

If you'd like to try the app outside of a container first, run:

```
cd src
poetry install
poetry run python manage.py makemigrations
poetry run python manage.py migrate
poetry run python manage.py runserver
```

Then point your browser at http://localhost:8000/


https://login.microsoftonline.com/8a791446-3f74-41af-be7d-470e2f985275/saml2?SAMLRequest=jZFRS8MwFIX%2FSonPa5OuozG0hWzdYDBBNvXBt0u9ukKT1Nx0ir%2FermNPgvp6uedwvnMKAtP1Sg%2FhaPf4PiCF6NN0lko2eKscUEvKgkFSoVEHfbdTacyVwQAvEIBF27pkG5nVUkqt58ssW4mlzLJ5vtDZWqaC17drFj2hp9bZko3iUUM04NZSABvGE0%2FTmeAzLh64VIKrBY9znj%2Bf%2F%2B6BqD1hyV6hI2SRJkIfRqeVszQY9Af0p7bBx%2F2uZMcQelJJQu2bbW0MHxSDgS9n48aZ5AzKLmxqgv6dsPcuuMaNko3zDU4FXWNUxUTg%2F9MUXBOz6u98N0IUycW7KpKf01Tf



https://login.microsoftonline.com/8a791446-3f74-41af-be7d-470e2f985275/saml2?SAMLRequest=jZFRS8MwFIX%2FSonPa5O2wyy0hWzdYDBBNvXBt0u9ukKT1Nx0ir%2FermNPgvp6uedwvnMKAtP1Sg%2FhaPf4PiCF6NN0lko2eKscUEvKgkFSoVEHfbdTacyVwQAvEIBF27pkG5nXUkqts2Wer8RS5nl2O9f5WqaC14s1i57QU%2BtsyUbxqCEacGspgA3jiafpTPAZFw98oQRX6TyWmXg%2B%2F90DUXvCkr1CR8giTYQ%2BjE4rZ2kw6A%2FoT22Dj%2FtdyY4h9KSShNo329oYPigGA1%2FOxo0zyRmUXdjUBP07Ye9dcI0bJRvnG5wKusaoionA%2F6cpuCZm1d%2F5boQokot3VSQ%2Fp6m%2BAQ%3D%3D



tenant id: 8a791446-3f74-41af-be7d-470e2f985275# msd-poc
# msd-poc
