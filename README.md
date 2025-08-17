# CoSyLab Website

This repository contains the **CoSyLab Website**, including:

* Main user-facing frontend (`./CoSyLab_Final`)
* Admin portal frontend (`./adminportal/frontend`)
* Backend API (`./adminportal/Backend`)

---

## Tech Stack

* Frontend: React (Vite)
* Backend: Node.js + Express
* Utilities: bcrypt, concurrently, cross-env, kill-port

---

## Project Structure

CoSylab/
├── Cosylab/         
   ├── Cosylab\_Final/      # Main frontend
├── adminportal/
│   ├── frontend/           # Admin portal frontend
│   └── Backend/            # Backend API
├── package.json
└── README.md

---

## Installation

1. Clone the repository:
   git clone [https://github.com/aman22060/CoSylab.git](https://github.com/aman22060/CoSylab.git)
   cd CoSyLab

2. Install dependencies:
   npm install
   npm install --prefix ./CoSyLab\_Final
   npm install --prefix ./adminportal/frontend
   npm install --prefix ./adminportal/Backend

---

## Development

Run frontend (main site only):
npm run dev\:main

Run admin portal (frontend only):
npm run dev\:admin

Run backend (API only):
npm run dev\:api

Run everything concurrently:
npm run dev\:all

This starts all services at once:

* Main site → [http://localhost:5173](http://localhost:5173)
* Admin portal → [http://localhost:3000](http://localhost:3000)
* Backend API → [http://localhost:3005](http://localhost:3005)

---

## Build

Build main frontend:
npm run build\:main

Build admin frontend:
npm run build\:admin

Build all frontends:
npm run build\:all

---

## Notes

* Ports are automatically freed before starting (via kill-port).
* Stop all running processes with Ctrl + C.
* For quick development, prefer:
  npm run dev\:all
* Add Admin password variables (if required) in `.env` inside the backend folder else the password is adminaccess123
