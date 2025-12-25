Overview

This project is a prototype of a Signature Injection Engine designed to solve a core problem in digital document signing:

Ensuring that a signature placed in a browser appears in the exact same location in the final, signed PDF — regardless of screen size, device, or resolution.

The system bridges the gap between:

Frontend browsers (CSS pixels, top-left origin, responsive)

PDF files (points, bottom-left origin, fixed layout)

The result is a reliable, auditable, and explainable PDF signing flow similar to what is used in products like BoloForms.

Key Features

Responsive PDF editor (Desktop → Mobile safe)

Drag & resize signature fields

Percentage-based coordinate system

Pixel-perfect PDF burn-in

Aspect-ratio safe signature rendering

SHA-256 audit trail (before & after signing)

Simple, explainable math and logic

Tech Stack
Frontend

React.js

react-pdf (PDF.js)

react-rnd (drag & resize)

Backend

Node.js

Express.js

pdf-lib

Native crypto (SHA-256)

Project Structure
signature-injection-engine/
│
├── frontend/
│   ├── src/
│   │   └── App.jsx
│   ├── public/
│   │   └── sample.pdf
│   └── package.json
│
├── backend/
│   ├── server.js
│   └── sample.pdf
│
└── README.md
