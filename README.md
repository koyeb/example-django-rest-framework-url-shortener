<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Deploy a Django REST Framework URL Shortener on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>

## About Koyeb and the URL Shortener built with Django REST Framework example application

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management.
This repository contains a Django REST Framework URL Shortener you can deploy on the Koyeb serverless platform for testing.

This example application is designed to show how a Django REST URL Shortener can be deployed on Koyeb.

## Getting Started

Follow the steps below to deploy and run the Django REST URL Shortener on your Koyeb account.

### Requirements

You need a Koyeb account to successfully deploy and run this application. If you don't already have an account, you can sign up for free [here](https://app.koyeb.com/auth/signup).

## Deploy using the Koyeb button

The fastest way to deploy the Django REST URL Shortener is to click the "Deploy to Koyeb" button.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=url-shortener&type=git&repository=koyeb/example-django-rest-framework-url-shortener&branch=main&builder=buildpack&run_command=gunicorn%20urlshortener.wsgi&env[DATABASE_URL]=REPLACE_ME&env[DISABLE_COLLECTSTATIC]=1&env[DJANGO_ALLOWED_HOSTS]=REPLACE_ME)

### Fork and deploy to Koyeb

If you want to customize and enhance this application, you need to fork this repository.

On the [Koyeb Control Panel](//app.koyeb.com/apps), on the **Overview** tab, click the **Create Web Service** button to begin.

1. Select `GitHub` as the deployment method.
2. In the repositories list, select the repository you just forked.
3. Expand the **Builder** section. Click the **override** toggle associated with the **Run command** and enter `gunicorn url_project.wsgi` in the field.
4. In the **Environment variables** section, click **Add variable** to add variables for `DATABASE_URL` with `?sslmode=require` added at the end, `DISABLE_COLLECTSTATIC` with the value `1`, and `DJANGO_ALLOWED_HOSTS` with the value `<YOUR_APP_NAME>-<YOUR_KOYEB_ORG>.koyeb.app`.
5. Then, give your App a name, i.e `url-shortener`, and click `Deploy`.

You land on the deployment page where you can follow the build of your application. Once the build is completed, your application is being deployed and you will be able to access it via `<YOUR_APP_NAME>-<YOUR_ORG_NAME>.koyeb.app`.

## Contributing

If you have any questions, ideas or suggestions regarding this application sample, feel free to open an [issue](//github.com/koyeb/example-django-rest-framework-url-shortener/issues) or fork this repository and open a [pull request](//github.com/koyeb/example-django-rest-framework-url-shortener/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)
