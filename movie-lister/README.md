# Movie Lister Application

A modern movie management application built with ES6+ JavaScript classes and modules. This project demonstrates object-oriented programming, local storage persistence, and modular JavaScript architecture for managing a personal movie collection.

## 🚀 Features

- **Add Movies** - Add movies with title, director, and URL
- **List Movies** - Display all movies in a organized table
- **Delete Movies** - Remove movies from the collection
- **Local Storage** - Persistent data across browser sessions
- **ES6+ Classes** - Object-oriented programming approach
- **Modular Architecture** - Separated concerns with different modules
- **Form Validation** - Input validation before adding movies
- **Responsive UI** - Clean Bootstrap-based interface
- **CRUD Operations** - Full Create, Read, Delete functionality

## 📁 Project Structure

```
movie-lister/
├── index.html          # Main HTML structure
├── film.js             # Film class definition
├── project.js          # Main application logic
├── ui.js               # UI manipulation methods
├── storage.js          # Local storage operations
└── README.md           # Project documentation
```

## 🛠️ Technologies Used

- HTML5
- Bootstrap 4
- Vanilla JavaScript (ES6+)
- ES6 Classes
- ES6 Modules
- Local Storage API
- Object-Oriented Programming

## 🌐 Live Demo

Visit the repository: [web-development-starter-kit](https://github.com/mirhatfidan/web-development-starter-kit)

## 💻 Getting Started

### Prerequisites

- A modern web browser with ES6+ support
- No additional dependencies required!

### Installation

1. Clone the repository:
```bash
git clone https://github.com/mirhatfidan/web-development-starter-kit.git
```

2. Navigate to the project directory:
```bash
cd web-development-starter-kit/movie-lister
```

3. Open `index.html` in your browser:
   - Double-click the file, or
   - Use a local development server (Live Server in VS Code)

## 📸 Screenshots

_A modern movie management application with ES6 classes and modular architecture._

## 🎯 Learning Objectives

This project was created to practice and demonstrate:

- **ES6+ Classes** - Object-oriented programming in JavaScript
- **Module Pattern** - Separating concerns and organizing code
- **Constructor Functions** - Creating object instances
- **Class Methods** - Defining class behaviors
- **Local Storage** - Persisting data in the browser
- **CRUD Operations** - Create, Read, Delete operations
- **Form Handling** - Processing user input
- **DOM Manipulation** - Dynamic UI updates
- **Event Delegation** - Efficient event handling

## 🎨 Application Architecture

### Film Class (`film.js`)
```javascript
class Film {
  constructor(title, director, url)
  // Represents a movie object
}
```

### Storage Module (`storage.js`)
- `getFilms()` - Retrieve movies from local storage
- `addFilm()` - Save new movie to local storage
- `deleteFilm()` - Remove movie from local storage

### UI Module (`ui.js`)
- `addFilmToUI()` - Display movie in the table
- `clearInputs()` - Reset form fields
- `deleteFilmFromUI()` - Remove movie from display
- `showAlert()` - Display user notifications

### Project Module (`project.js`)
- Main application logic
- Event listeners
- Coordination between modules

## 🔧 How It Works

1. **Add Movie**: User fills form with movie details
2. **Create Instance**: Film class instance is created
3. **Save**: Movie is saved to local storage via Storage module
4. **Display**: UI module updates the table with new movie
5. **Delete**: User can remove movies from collection
6. **Persist**: All changes are saved to local storage

## 📦 Key JavaScript Concepts

- **ES6 Classes** - Modern OOP syntax
- **Constructor Methods** - Object initialization
- **Static Methods** - Class-level methods
- **Module Pattern** - Code organization
- **Local Storage API** - Data persistence
- **JSON Methods** - Parse and stringify
- **Array Methods** - forEach, filter, find
- **Event Listeners** - User interaction handling

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

- Group collaboration project
- Part of web development coursework - ES6+ JavaScript practice
- Thanks to all team members (Mirhat & Ekin) for their contributions
- Focus on modern JavaScript and OOP principles

---

⭐ Star this repository if you found it helpful!

