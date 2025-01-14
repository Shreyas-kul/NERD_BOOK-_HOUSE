# NERD_BOOK-_HOUSE
# Library Management System

## Project Description
The **Library Management System** is a console-based application that allows users to manage a collection of books, including both physical and digital formats (eBooks). The program provides functionalities such as adding, deleting, searching, updating, checking out, and returning books. It also supports persistent storage using a text file to save and load book data.

---

## Features

1. **Add Books**
   - Add physical books or eBooks by providing details like title, author, ISBN, quantity, file format (for eBooks), and file size (for eBooks).

2. **Delete Books**
   - Remove a book from the collection using its ISBN.

3. **Search Books**
   - Find a book by its ISBN and display its details.

4. **Update Book Details**
   - Modify a book's title, author, and quantity using its ISBN.

5. **Check Out Books**
   - Reduce the quantity of a book when it is checked out.

6. **Return Books**
   - Increase the quantity of a book when it is returned.

7. **Display Out of Stock Books**
   - List all books with a quantity of zero.

8. **Display All Books**
   - Show details of all books in the library.

9. **Persistent Storage**
   - Save all book data to a file (`library_data.txt`) for future use.

---

## How to Run

1. **Prerequisites**
   - C++ Compiler (e.g., GCC or Clang)
   - A text editor or IDE (e.g., Visual Studio Code, CLion)

2. **Compiling the Code**
   - Open a terminal or command prompt.
   - Navigate to the directory containing the source code file.
   - Run the following command to compile:
     ```
     g++ -o library_management library_management.cpp
     ```

3. **Running the Program**
   - Execute the compiled program:
     ```
     ./library_management
     ```

---

## File Format for `library_data.txt`
The data is saved in the following format:
- **Physical Book:**
  ```
  Book,<ISBN>,<Quantity>,<Title>,<Author>
  ```
- **EBook:**
  ```
  EBook,<ISBN>,<Quantity>,<Title>,<Author>,<File Format>,<File Size>
  ```

### Example
```
Book,1234567890,5,The Great Gatsby,F. Scott Fitzgerald
EBook,9876543210,3,Digital Fortress,Dan Brown,PDF,2.5
```

---

## Program Structure

### Classes

1. **Book**
   - Base class representing a generic book.
   - Contains attributes like title, author, ISBN, and quantity.

2. **EBook**
   - Derived class representing an eBook.
   - Additional attributes: file format and file size.

3. **Library**
   - Manages a collection of books.
   - Handles file operations (saving and loading), and provides various management functionalities.

---

## Usage

Upon running the program, the user will be presented with a menu to select various options. For example:

```
WELCOME TO NERD BOOK HOUSE
1. Add Book
2. Delete Book
3. Search Book
4. Update Book Details
5. Check Out Book
6. Return Book
7. Display Out of Stock Books
8. Display All Books
9. Exit
Enter your choice:
```

Users can interact with the program by entering the corresponding option number and following the prompts.

---

## Future Enhancements
- Add user authentication for librarians and members.
- Support for borrowing limits and due dates.
- Enhanced UI using a GUI framework.
- Support for different file formats (e.g., JSON or XML) for data storage.

---

## License
This project is open-source and free to use and modify. Contributions are welcome!

