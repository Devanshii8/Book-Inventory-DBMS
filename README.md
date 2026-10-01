# Book Inventory DBMS

A web-based application to manage book inventories efficiently. This system enables users to add, update, delete, and search for books within the inventory while ensuring data consistency and reliability.

## Features

- **CRUD Operations:**
  - Create, Read, Update, and Delete book records.
- **Search Functionality:**
  - Search for books by title, author, or genre.
- **Database Integration:**
  - Efficiently handles large inventories using PostgreSQL.
- **Responsive Design:**
  - User-friendly interface built with HTML, CSS, and JavaScript.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js, Express.js
- **Database:** PostgreSQL (PLpgSQL)

## Installation

Follow these steps to set up the project locally:

1. **Clone the Repository:**
   ```bash
  git clone https://github.com/Devanshii8/Book-Inventory-DBMS.git
   cd Book_Inventory_DBMS
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Setup Database:**
   - Ensure PostgreSQL is installed on your machine.
   - Create a database named `book_inventory`.
   - Import the schema from `schema.sql` into your database:
     ```bash
     psql -U [username] -d book_inventory -f schema.sql
     ```

4. **Configure Environment Variables:**
   - Create a `.env` file in the project root and add the following:
     ```env
     DB_HOST=localhost
     DB_USER=[your_postgres_username]
     DB_PASSWORD=[your_postgres_password]
     DB_NAME=book_inventory
     DB_PORT=5432
     ```

5. **Run the Application:**
   ```bash
   npm start
   ```

6. **Access the Application:**
   - Open your browser and navigate to `http://localhost:3000`.

## Usage

1. **Add Books:** Fill out the form to add a new book to the inventory.
2. **Edit Books:** Click the edit icon to update book details.
3. **Delete Books:** Click the delete icon to remove a book from the inventory.
4. **Search Books:** Use the search bar to find specific books by title, author, or genre.



## Project Structure

```
Book_Inventory_DBMS/
├── public/
│   ├── css/
│   ├── js/
├── routes/
├── views/
├── app.js
├── schema.sql
├── package.json
├── .env
```

## Challenges and Solutions

1. **Data Consistency:**
   - Implemented proper transaction handling to maintain data integrity.
2. **Scalability:**
   - Designed the database schema with indexing for faster queries on large datasets.
3. **Security:**
   - Added input sanitization to prevent SQL injection and other security threats.

## Future Enhancements

- **Advanced Filtering:**
  - Implement advanced filters for searching books.
- **API Integration:**
  - Expose RESTful APIs for external applications.

## Contributing

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

For any queries, please contact:

- **Name:** Devanshi Gupta
- **GitHub:** https://github.com/Devanshii8

---

Thank you for checking out the Book Inventory DBMS project!
