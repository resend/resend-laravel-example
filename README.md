# Resend with Laravel

This example shows how to use Resend with [Laravel](https://laravel.com).

## Prerequisites

To get the most out of this guide, you’ll need to:

* [Create an API key](https://resend.com/api-keys)
* [Verify your domain](https://resend.com/domains)

## Instructions

1. Install the `composer` and `npm` dependencies:

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
