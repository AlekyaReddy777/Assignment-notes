
Notes App
Objective
Build a Simple Notes App using the specified tech stack. The application should allow users to efficiently create, update, and organise notes.

Tech Stack
Frontend: React.js, React Router DOM
Backend: Node.js, Express.js
Database: SQLite

Features and Flow
1. User Authentication
Implement user signup and login functionality.
Store hashed passwords securely.
Use JWT for authentication.
After successful login, redirect users to the dashboard.

2. Dashboard
Display a list of notes with the following details:
Title
Content
Created Date
Last Updated Date
Category (Personal, Work, Study, Others)
Allow users to:
Add new notes
Edit existing notes (title, content, category).
Delete notes.
Search notes by title or content.
Filter notes by category.

3. Note Management
Users should be able to:
View all notes in a table or card format.
Click on a note to view its details.
Pin important notes (Pinned notes appear at the top).
Mark a note as archived (Move to an archive section instead of deleting).
Restore archived notes back to active notes.

4. Database Design (SQLite)
Users Table
Column
Type
Description
id
INTEGER (Primary Key)
Unique User ID
name
TEXT
User's Name
email
TEXT (Unique)
User's Email
password
TEXT
Hashed Password
created_at
DATETIME
Account Created Time

Notes Table
Column
Type
Description
id
INTEGER (Primary Key)
Unique Note ID
title
TEXT
Note Title
content
TEXT
Note Content
category
TEXT
Personal, Work, Study, etc.
created_at
DATETIME
Date Created
updated_at
DATETIME
Last Modified Date
pinned
BOOLEAN
If the note is pinned
archived
BOOLEAN
If note is archived
user_id
INTEGER (Foreign Key)
References Users Table


5. API Endpoints
User Authentication
POST /signup – Register a user.
POST /login – Authenticate user and return JWT token.
Note Management
GET /notes – Fetch all notes for a user.
POST /notes – Create a new note.
PUT /notes/:id – Update a note.
DELETE /notes/:id – Delete a note.
PATCH /notes/:id/pin – Pin/unpin a note.
PATCH /notes/:id/archive – Archive/unarchive a note.

Bonus (Optional)
✅ Implement search and filter functionality for notes.
✅ Add pagination for note lists.
✅ Use httpOnly cookies for secure authentication.
✅ Deploy the application online.

Evaluation Criteria
Proper usage of the tech stack.
Secure authentication & authorization.
Well-structured code architecture.
Clean UI/UX.
Efficient database design.
Proper error handling.

Deployment
Deploy the backend (e.g., Render).
Deploy the frontend (e.g., Vercel, Netlify).
Provide a Postman collection for API testing.

Assignment Submission Guidelines
Submit your GitHub Repository link 
Submit your deployed application link.
Submit a Loom video recording explaining your project Code & output and functionality.
