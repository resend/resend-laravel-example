<div align="left">
    <picture>
        <source srcset="https://user-images.githubusercontent.com/68016351/221072893-61d9e99a-ed2a-4f58-b167-0ff2cbea0614.svg" media="(prefers-color-scheme: dark)" height="32">
        <img src="https://user-images.githubusercontent.com/68016351/221070388-c5faf78a-d3b7-440b-a300-c2e7b635279b.svg" height="32">
    </picture>
   <p>Resend is the email platform for developers.</p>
</div>

---

This is a sample project demonstrating how to integrate [Resend for Laravel](https://github.com/resendlabs/resend-laravel) into a Laravel 10 application, based on [Laravel Bootcamp](https://bootcamp.laravel.com/)'s Blade implementation of Chirper.

> **Note**
> The integration for Laravel 9 is identical.

## Introduction

This sample 

## Getting started

1. Clone this repository:

```bash
git clone https://github.com/resendlabs/resend-laravel-example.git resend-laravel-example
```

2. Set the work directory to the example project:

```bash
cd resend-laravel-example
```

3. Install the `composer` and `npm` dependencies:

```bash
composer install && npm install
```

4. Build the Javascript and CSS files required for the frontend:

```bash
npm run build
```

5. Create a `.env` file used to configure your application:

```bash
php -r "file_exists('.env') || copy('.env.example', '.env');"
```

6. Generate an application key:

```bash
php artisan key:generate --ansi
```

7. Configure your `.env` file, with your database credentials and [Resend API key](https://resend.com/api-keys).

8. Migrate the database:

```bash
php artisan migrate
```

9. You're ready to use the example project, run:

```bash
php artisan serve
```

### Using the example app

To get the full experience of how easy it is to send emails with Resend, follow these simple steps:

1. Create two user accounts with valid email addresses.
2. Once you have two user accounts, login into any one of them and navigate to the "Chirps" page.
3. Write your very first Chirp.
4. Once you have submitted your first Chirp, the application will use Resend to email all users of your new Chirp.
5. If you used a valid email address you should receive an email in your inbox or you can check your [Resend dashboard](https://resend.com/emails) to view the sent email.
