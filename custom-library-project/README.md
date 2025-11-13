# Custom Library Project

A comprehensive library management system built with vanilla JavaScript, featuring two different implementation approaches: **Constructor/Prototype Pattern** and **ES6 Class Pattern**. This project demonstrates object-oriented programming concepts, local storage persistence, and modern JavaScript development practices.

## 🚀 Features

- **Book Management** - Add, list, and delete books
- **Two Implementations** - Compare Prototype vs Class patterns
- **Local Storage** - Persistent book data across sessions
- **Book Images** - Visual representation of books
- **Form Validation** - Validate book information before adding
- **Search Functionality** - Find books by title or author
- **Responsive UI** - Clean and user-friendly interface
- **Real-time Updates** - Instant UI updates on actions
- **Error Handling** - User-friendly alerts and notifications

## 📁 Project Structure

```
custom-library-project/
├── prototype/              # Constructor/Prototype Pattern Implementation
│   ├── index.html         # Main HTML file
│   ├── app.js             # Main application logic
│   ├── library.js         # Book constructor and prototype methods
│   ├── ui.js              # UI manipulation module
│   ├── storage.js         # Local storage operations
│   ├── style.css          # Styling
│   └── assets/            # Book cover images
│       ├── 1984.jpg
│       ├── simyaci.jpg
│       ├── prens.jpg
│       ├── ermis.jpg
│       └── bg.jpg
├── classlib/              # ES6 Class Pattern Implementation
│   ├── index.html         # Main HTML file
│   ├── app.js             # Main application logic
│   ├── library.js         # Book class definition
│   ├── ui.js              # UI class
│   ├── storage.js         # Storage class
│   ├── style.css          # Styling
│   └── assets/            # Book cover images
└── README.md              # Project documentation
```

## 🛠️ Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript (ES5 & ES6+)
- Local Storage API
- Constructor Functions & Prototypes
- ES6 Classes
- Module Pattern
- Object-Oriented Programming

## 🌐 Live Demo

Visit the repository: [web-development-starter-kit](https://github.com/mirhatfidan/web-development-starter-kit)

## 💻 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies required!

### Installation

1. Clone the repository:
```bash
git clone https://github.com/mirhatfidan/web-development-starter-kit.git
```

2. Navigate to the project directory:
```bash
cd web-development-starter-kit/custom-library-project
```

3. Choose an implementation:
   - **Prototype Version**: Open `prototype/index.html`
   - **Class Version**: Open `classlib/index.html`

## 📸 Screenshots

_A modern library management system with book covers and organized interface._

## 🎯 Learning Objectives

This project was created to practice and demonstrate:

- **OOP Principles** - Encapsulation, abstraction, modularity
- **Constructor Functions** - Creating objects with constructors
- **Prototype Pattern** - Adding methods to prototype
- **ES6 Classes** - Modern class syntax
- **Static Methods** - Class-level methods
- **Module Pattern** - Separating concerns
- **Local Storage** - Browser storage operations
- **CRUD Operations** - Create, Read, Delete
- **Form Handling** - User input validation
- **DOM Manipulation** - Dynamic UI updates

## 🎨 What You Can Do

### 1. Add Books
- Fill in the book form with:
  - **Book Title** - Name of the book
  - **Author** - Book author's name
  - **ISBN** - International Standard Book Number
  - **Book Image** - Cover image URL or select from presets
- Click "Add Book" to save to library
- Book appears instantly in the list
- Data saved to local storage automatically

### 2. View Book Collection
- See all books displayed as cards
- Each card shows:
  - Book cover image
  - Title and author information
  - ISBN number
  - Delete button
- Books persist even after browser refresh
- Organized grid layout for easy browsing

### 3. Delete Books
- Click the "X" button on any book card
- Book is removed from both UI and storage
- Confirmation message displays
- Remaining books reorganize automatically

### 4. Search & Filter (Can be extended)
- Search by title or author
- Filter by genre or year
- Sort books alphabetically

### 5. Edit Book Information (Can be extended)
- Update book details
- Change cover image
- Modify author or ISBN

## 🔧 Implementation Comparison

### Prototype Pattern (`prototype/`)
```javascript
// Constructor Function
function Book(title, author, isbn, image) {
  this.title = title;
  this.author = author;
  this.isbn = isbn;
  this.image = image;
}

// Prototype Methods
Book.prototype.getBookInfo = function() {
  return `${this.title} by ${this.author}`;
};

// Storage using function-based module
const Storage = {
  getBooks: function() { /* ... */ },
  addBook: function(book) { /* ... */ }
};
```

**Advantages:**
- Compatible with older browsers
- Memory efficient (methods shared via prototype)
- Traditional JavaScript approach
- Good for understanding JavaScript fundamentals

### Class Pattern (`classlib/`)
```javascript
// ES6 Class
class Book {
  constructor(title, author, isbn, image) {
    this.title = title;
    this.author = author;
    this.isbn = isbn;
    this.image = image;
  }
  
  getBookInfo() {
    return `${this.title} by ${this.author}`;
  }
}

// Storage Class
class Storage {
  static getBooks() { /* ... */ }
  static addBook(book) { /* ... */ }
}
```

**Advantages:**
- Modern, cleaner syntax
- Easier to read and maintain
- Built-in static methods
- Industry standard approach

## 📦 Key Features Explained

### Book Object Structure
```javascript
{
  title: "1984",
  author: "George Orwell",
  isbn: "978-0451524935",
  image: "assets/1984.jpg"
}
```

### Local Storage Operations
- **Save Books**: Store array as JSON
- **Retrieve Books**: Parse JSON from storage
- **Update Books**: Modify and re-save
- **Delete Books**: Filter and update storage

### UI Components
- **Add Form**: Input fields with validation
- **Book List**: Dynamic card grid
- **Alert System**: Success/error messages
- **Delete Buttons**: Individual remove actions

## 🚀 Advanced Features You Can Add

1. **Book Categories** - Organize by genre
2. **Rating System** - Rate books 1-5 stars
3. **Reading Status** - Track read/unread books
4. **Notes Section** - Add personal notes
5. **Export Data** - Download library as JSON/CSV
6. **Import Books** - Upload book data
7. **Search Bar** - Real-time search
8. **Sort Options** - By title, author, date added
9. **Dark Mode** - Theme switcher
10. **Book Details Page** - Expanded view with description

## 🎓 Technical Concepts Demonstrated

### 1. Object-Oriented Programming
- Encapsulation of book data
- Separation of concerns (UI, Storage, Logic)
- Reusable code structure

### 2. Data Persistence
- Local Storage API usage
- JSON serialization/deserialization
- State management across sessions

### 3. Event Handling
- Form submission events
- Delete button clicks
- Input validation

### 4. DOM Manipulation
- Creating elements dynamically
- Updating UI in real-time
- Removing elements

### 5. Error Handling
- Form validation
- Empty field checks
- User feedback messages

## 🤝 Contributing

This is a learning project, but suggestions and improvements are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is created for educational purposes.

## 👨‍💻 Author

**Mirhat Fidan**

- GitHub: [@mirhatfidan](https://github.com/mirhatfidan)

## 🙏 Acknowledgments

- Part of web development coursework - JavaScript OOP project
- Thanks to all team members for their contributions
- Focus on comparing programming patterns
- Emphasis on practical JavaScript applications

## 📚 Learning Resources

- [MDN Web Docs - Prototypes](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object_prototypes)
- [MDN Web Docs - Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
- [JavaScript.info - Prototypes](https://javascript.info/prototypes)
- [JavaScript.info - Classes](https://javascript.info/classes)

---

⭐ Star this repository if you found it helpful!

