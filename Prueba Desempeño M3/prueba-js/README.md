# SPA Events App

This project is a Single Page Application (SPA) for managing and enrolling in events. It features user authentication, role-based access (admin and visitor), event creation and management, and enrollment functionality. The backend is powered by `json-server` for quick prototyping and development.

## Features

- User authentication (login, logout, register)
- Role-based dashboard (admin and visitor)
- Admins can create, edit, and delete events
- Visitors can view events and enroll if spots are available
- My Events section for visitors to see their enrollments
- Responsive and modern UI

## Technologies Used

- JavaScript (ES6+)
- HTML5 & CSS3
- [json-server](https://github.com/typicode/json-server) (mock REST API)

## Project Structure

```
├── app/
│   ├── auth.js
│   ├── router.js
│   ├── css/
│   │   ├── login.css
│   │   └── styles.css
│   └── views/
│       ├── create-event.js
│       ├── dashboard.js
│       ├── edit-event.js
│       ├── enrollments.js
│       ├── login.js
│       ├── my-events.js
│       ├── notFound.js
│       ├── register.js
│       └── visitor.js
├── auth.js
├── db.json
├── index.html
├── index.js
├── package.json
└── README.md
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) installed

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Salito112/prueba-js.git
   cd prueba-js
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Running the App

1. Start the mock API server:
   ```bash
   npm run json-server
   ```
   This will start `json-server` at [http://localhost:3000](http://localhost:3000).

2. Open `index.html` in your browser (use Live Server or similar extension for best SPA experience).

## Usage

- **Register** as a new visitor or **login** as an existing user (admin or visitor).
- **Admins** can manage events (create, edit, delete).
- **Visitors** can view all events, enroll in available events, and see their enrolled events in "My Events".

## Example Users

See `db.json` for predefined users:

- **Admin:**
  - Username: `admin`
  - Password: `admin123`
- **Visitor:**
  - Username: `Emanuel`
  - Password: `emanuel123`
