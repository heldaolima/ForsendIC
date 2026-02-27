# ForsendIC — Form Management System 📋

This repository contains the source code for **ForsendIC**, a web application built with Laravel in collaboration with the secretarial staff of the Computer Science Institute at the Federal University of Alagoas.
The main goal is to provide an organized platform to store, manage, and track the forms students need to fill out for the university's administrative requirements.

---

## Project Purpose

ForsendIC was born from a real need: to digitize and streamline the flow of academic and administrative forms that students of the Computer Science Institute frequently submit.
Before the project, the secretarial offices handled these documents manually, which generated a large volume of paper, delays, and rework.

Today the system allows:

- Centralized registration of forms completed by students;
- Viewing history by student ID, form type, and status;
- Notifications to the secretariat about new submissions or status changes;
- A simple, responsive interface for students and staff.

Development was carried out in direct partnership with the administrative team, ensuring that each feature met their actual needs.

---

## Key Features

1. **User authentication** (students, secretaries, administrators).
2. **Registration and management of forms** by type (declarations, requests, etc.).
3. **Document upload** and PDF generation.
4. **Approval workflow** with statuses: submitted, approved, rejected.
5. **OTP system** for identity confirmation during submission.
6. **Administrative dashboards** for managing users and forms.
7. **Email notifications** using customizable templates.
8. **Secure REST API** for future integrations.

---

## Technologies Used

- **PHP 8+** with **Laravel 10**
- **MySQL** database (via Eloquent ORM)
- Authentication and authorization with **Laravel Sanctum**
- Front-end using Blade + responsive Bootstrap
- **Redis** for cache and queues (optional)
- Email delivery via **Mailgun / SMTP**
- Automated tests with **PHPUnit**
- Version control with **Git**

---

## Installing and Running the Application

1. **Clone the repository**

```bash
git clone https://github.com/your-username/ForsendIC.git
cd ForsendIC
```

2. **Install dependencies**

```bash
composer install
npm install && npm run dev
```

3. **Configure the environment**

- Copy `.env.example` to `.env`.
- Adjust `DB_*`, `MAIL_*` and other variables according to your environment.
- Generate the application key: `php artisan key:generate`.

4. **Migrate the database**

```bash
php artisan migrate --seed
```

5. **(Optional) Run queues and clear cache**

```bash
php artisan queue:work
php artisan cache:clear
```

6. **Start the server**

```bash
php artisan serve
```

Visit [http://localhost:8000](http://localhost:8000) and create an account to test.

---

## Contributions

This project is the result of an open collaboration. Any student or community member can contribute by
opening issues or pull requests following the [Laravel style conventions](https://laravel.com/docs/10.x/contributions).

---

## License

This code is available under the **MIT license**.

---
