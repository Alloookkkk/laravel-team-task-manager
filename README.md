Laravel Team Task Manager
    A small but complete Laravel application where a user can create companies, add projects under each company, and manage tasks for every project with statuses, priorities, and due dates.
Built with Laravel.
​

Project Overview
    This project is a portfolio-ready Laravel app built to practice real-world CRUD operations, nested resources, authorization, and database seeding. A logged-in user can manage a simple hierarchy: Company → Projects → Tasks, and filter tasks by status (todo, in progress, done). The structure and code style are intentionally close to production so it can be discussed in interviews as an example of backend and basic UI skills.
​

Features
    (1)Company management: create, edit, delete companies.
    (2)Projects nested under a company with their own CRUD operations.
    (3)Tasks nested under a project with title, description, status, priority, and due date.
    (4)Status filter buttons on the task list (All, To do, In progress, Done).
    ​(5)Simple authorization so users only access their own companies, projects, and tasks.
    (6)Database seeders and factories to generate demo data quickly.
​

Tech Stack
    Backend: Laravel (latest version used in this project).
    Language: PHP.
    Database: MySQL (or any Laravel-supported database via configuration).
    Frontend: Blade templates with utility-style classes and inline styling.
    Tooling: Vite, Node.js, npm for asset bundling.

Getting Started
    Prerequisites
    Install these tools first:
        (1)PHP (compatible with this Laravel version).
​        (2)Composer.
​        (3)Node.js and npm.
​        (4)MySQL (or another supported database such as             PostgreSQL or SQLite).
​        (5)Git (optional but recommended for version control).
​

    Installation
   (1)Clone the repository:

    git clone https://github.com/Alloookkkk/laravel-team-task-manager.git
    cd laravel-team-task-manager
    
    (2)Install PHP dependencies:

    composer install

    (3)Copy the example environment file and configure it:

    cp .env.example .env
    Update the database name, username, and password in .env under the DB_ settings.
​

    (4)Generate the application key:

    php artisan key:generate
    
    (5)Run migrations and seeders (this will also create demo data):
    
    php artisan migrate:fresh --seed

    (6)Install frontend dependencies and build assets:

    npm install
    npm run dev
    
    (7)Start the Laravel development server:

    php artisan serve
    The app will be available at http://127.0.0.1:8000 by default.
​

Demo Login
    If your seeders create a demo user, document it here (adjust to match your actual seeder):

        Email: demo@example.com
        Password: password

    After logging in:

        Create a company.
        Add one or more projects under the company.
        Add tasks under a project and set status, priority, and due date.
        Use the filter buttons on the tasks page to view tasks by status.

    Project Structure (High Level)
        app/Models – Eloquent models for Company, Project, Task, and User.
        app/Http/Controllers – Controllers that handle company, project, and task logic.
        database/migrations – Database schema definitions for all tables.
        database/seeders – Seed classes to generate demo data and users.
        resources/views – Blade templates for companies, projects, and tasks UI.
        routes/web.php – Web routes for all pages and nested resources.
​

## Screenshots

![Dashboard](screenshots/dashboard.png)
![Your companies](screenshots/your-company-page.png)
![Projects](screenshots/project-page.png)
![Tasks](screenshots/task-page.png)
![Create company](screenshots/create-company-page.png)
![Create task](screenshots/task-create-page.png)
![Register](screenshots/register.png)
![Login](screenshots/login.png)
![Forgot password](screenshots/forgot-password.png)


