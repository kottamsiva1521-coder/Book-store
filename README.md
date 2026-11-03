# Bookstore CRUD Application

Frontend + backend using HTML/CSS/JavaScript, Node.js, Express, and MySQL.

## Database columns
`book_id`, `title`, `author`, `category`, `price`, `stock`

## Setup

1. Install Node.js (LTS) and MySQL Server (or use MySQL through XAMPP).
2. Open MySQL Workbench/phpMyAdmin or another MySQL client.
3. Run the contents of `database.sql` to create the `bookstore` database and `books` table.
4. Open this project folder in VS Code.
5. Copy `.env.example` to a new file named `.env`.
6. Edit `.env` and set `DB_USER` and `DB_PASSWORD` to your own MySQL credentials. Keep `.env` private.
7. Open a terminal in this folder and run:

   ```bash
   npm install
   npm start
   ```

8. Open **http://localhost:3000** in your browser. Use this URL, not `file://` or Live Server, so the frontend and API share the same origin.

## CRUD API
- `POST /books` — create a book
- `GET /books` — list all books
- `GET /books/:book_id` — read one book
- `PUT /books/:book_id` — update a book
- `DELETE /books/:book_id` — delete a book
- `GET /health` — server health check

## Notes
- Sample records for IDs 101 and 102 are included in `database.sql`. Remove the sample INSERT if you want an empty table.
- Book IDs must be unique. Price and stock cannot be negative.
- Do not commit or share your real `.env` file.
