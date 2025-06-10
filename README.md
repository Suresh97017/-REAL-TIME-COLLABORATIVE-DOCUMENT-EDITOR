# -REAL-TIME-COLLABORATIVE-DOCUMENT-EDITOR

COMPANY : CODTECH IT SOLUTIONS

NAME : DAKAMARRI SURESH

INTERN ID : CT04DF2473

DOMAIN : FULL STACK WEB DEVELOPMENT

DURATION : 4 WEEKS

MENTOR : NEELA SANTOSH

DESCRIPTION :

Real-Time Collaborative Text Editor :

This project is a real-time collaborative text editor developed using React.js for the frontend and Node.js with Socket.IO for the backend. The goal of this application is to allow multiple users to edit text in real time, with their changes immediately reflected on all connected clients. This functionality is similar to what is seen in collaborative tools like Google Docs.

The editor allows users to type, format, and style text using a rich text interface. It is built on top of Quill.js, which is a powerful, open-source rich text editor that supports a wide range of formatting options. These include bold, italics, underline, headings, lists, block quotes, and code blocks.

The frontend is created using React, a popular JavaScript library for building user interfaces. In the frontend, a component called TextEditor is responsible for rendering the Quill editor and handling socket communication. When a user types something in the editor, those changes are captured and emitted to the server using Socket.IO. Simultaneously, the editor also listens for changes coming from other users and updates the content accordingly in real time.

The backend of the application is powered by Node.js, using the Express.js framework to set up the server and integrate Socket.IO for real-time bi-directional communication between the server and all connected clients. When a user sends an update (like typing or formatting text), the server receives the changes and broadcasts them to all other users, ensuring synchronization of data across all clients.

Key Features:

Real-Time Collaboration:

As users type or format the text, their changes appear instantly for all other users.

This is made possible using WebSockets via the Socket.IO library, which maintains an open connection between the client and server.

Rich Text Editing:

The application uses Quill.js to provide a rich set of formatting tools.

Users can make text bold, italic, or underlined, as well as insert headers, lists, block quotes, and code snippets.

Seamless Synchronization:

All changes are tracked and sent only when the user makes them, reducing unnecessary traffic.

The changes are transmitted in the form of delta objects (Quill’s internal change format) and applied on other clients to keep everything in sync.

Clean Code Structure:

The project is organized into a clean directory structure with client/ for the frontend and server/ for the backend.

React components are separated logically, and Socket.IO integration is neatly handled using React hooks.

How it Works:

The user opens the text editor on their browser (http://localhost:3000).

The frontend creates a Quill editor instance and connects to the backend via Socket.IO.

When the user types, Quill detects the text changes and emits the changes (called deltas) to the server.

The server receives the deltas and broadcasts them to all other connected users.

Each client listens for incoming deltas and updates their own editor, ensuring that all clients remain in sync.

Conclusion:

This real-time collaborative text editor project demonstrates how frontend and backend technologies can be combined to build a live-syncing application. It is a great learning example for understanding how WebSockets work, how to use React with external libraries like Quill, and how to handle event-driven communication between clients and servers. The final product is a lightweight but powerful editor that can be extended into a full-fledged collaborative writing tool with features like storage, access control, and version history.

OUTPUT:
