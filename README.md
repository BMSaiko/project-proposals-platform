# Project Proposals Platform (DSOS)

🇬🇧 English · [🇵🇹 Português](README.pt.md)

> Laravel web platform managing internship and project proposals between students, teachers and companies.

> Formerly `dsos-grupo1-bombastico`.

| | |
|---|---|
| **Context** | CTESP — Service-Oriented Systems Development (DSOS) |
| **Year** | 2023/24 |
| **Team** | Group 1 |
| **Stack** | PHP · Laravel · MySQL · Blade · Bootstrap (Material Dashboard) · Composer · npm |

## What this project shows
- **MVC with Laravel**: models, controllers, Blade views, migrations and routes.
- Multi-role workflows (student, teacher, company) with state tracking.
- Database design (Laravel migrations).

## Features
- Registration, login and password recovery.
- Companies/teachers publish proposals; students apply, teachers apply as supervisors.
- Accept/reject applications; track proposal and application states.
- Project delivery (file submission) and feedback.
- Profile editing, company and student listings, application PDF.

## Structure
| Path | Content |
|---|---|
| `DSOS-grupo1-Bombastico/` | Laravel app (`app/Models`, `app/Http/Controllers`, `routes/web.php`, migrations) |

## Running
```bash
cd DSOS-grupo1-Bombastico
composer install
cp .env.example .env      # set DB credentials
php artisan key:generate
php artisan migrate
php artisan serve
```

## Notes
- `vendor/` and `.env` are not included.

## Documentation

- [Architecture, data model and known issues](docs/ARCHITECTURE.md)
- [Setup and troubleshooting](docs/SETUP.md)
- [ADR 0001 — Laravel MVC, roles by table](docs/adr/0001-laravel-mvc-roles-by-table.md)
