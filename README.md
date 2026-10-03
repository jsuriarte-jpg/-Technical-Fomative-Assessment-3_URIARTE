# CodeIgniter POS — TFA3

A four-page CodeIgniter 4 POS project with MySQL-backed customer and
user accounts, create and edit forms, validation, and staff avatars.

## Setup

1. Run `composer install`.
2. Copy `env` to `.env`.
3. Set the base URL and MySQL credentials in `.env`.
4. Import `database/pos_tfa3.sql` into MySQL once.
5. Run `php spark serve --port 8083`.
6. Visit `http://localhost:8083/`.

## Pages

- `/` — Home
- `/about` — About
- `/customers` — Customer Accounts
- `/users` — User Accounts

New accounts can be created from their listing pages. Existing accounts
have Edit links. A user's JPG or PNG avatar can be uploaded from the
Edit User page. Uploaded images are prepared as 160 × 160 thumbnails
in `public/uploads/avatars/`; the database stores only the filename.