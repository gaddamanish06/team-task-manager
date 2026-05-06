Team Task Manager - Full Stack Project

Live Application URL:
https://team-task-manager-production-fbeb.up.railway.app

GitHub Repository:
https://github.com/gaddamanish06/team-task-manager

Project Overview:
Team Task Manager is a full-stack web application where users can create projects, assign tasks, track task status, and manage team access using Admin and Member roles.

Key Features:
- Authentication with signup and login
- First registered user becomes Admin
- Later users become Members
- Project creation and team member management
- Task creation, assignment, status tracking, and deletion
- Dashboard with project totals, task totals, status counts, overdue tasks, and personal open tasks
- Role-based access control for Admins, Members, and project owners
- REST API backend with JSON document database storage

Tech Stack:
- Node.js HTTP server
- Vanilla JavaScript frontend
- HTML and CSS
- JSON NoSQL-style database stored in data/db.json
- Railway deployment

Local Setup:
1. Clone the repository.
2. Open the project folder.
3. Run npm install.
4. Run npm start.
5. Open http://localhost:3000.

Environment Variable:
JWT_SECRET should be configured in Railway for production authentication token signing.

API Routes:
- POST /api/auth/signup
- POST /api/auth/login
- GET /api/me
- GET /api/users
- PATCH /api/users/:id/role
- GET /api/projects
- POST /api/projects
- PATCH /api/projects/:id
- DELETE /api/projects/:id
- GET /api/tasks
- POST /api/tasks
- PATCH /api/tasks/:id
- DELETE /api/tasks/:id
- GET /api/dashboard

Demo Notes:
For the demo, create the first account as Admin, then show project creation, task assignment, task status updates, dashboard metrics, and team role management.
