# Library System

## Description

This project implements a simple library system using PHP and Object-Oriented Programming (OOP). It allows managing books, authors, users, and book loans. The system is composed of several classes that represent the different elements of the library domain.

## Classes

### Pessoa (Person)

- **Attributes:**
  - `nome`: string
  - `idade`: int

- **Methods:**
  - `__construct($nome, $idade)`: Constructor to initialize a person with name and age.
  - `getNome()`: Returns the person's name.
  - `getIdade()`: Returns the person's age.

### Autor (Author) - extends Pessoa

- **Attributes:**
  - `obras`: array

- **Methods:**
  - `adicionarObra($obra)`: Adds a work to the author's works array.
  - `listarObras()`: Returns an array with the author's works.

### Usuario (User) - extends Pessoa

- **Attributes:**
  - `livrosEmprestados`: array

- **Methods:**
  - `pegarLivro($livro)`: Adds a book to the user's borrowed books array and prints a message.
  - `devolverLivro($livro)`: Removes a book from the user's borrowed books array and prints a message.
  - `listarLivrosEmprestados()`: Returns an array with the books borrowed by the user.

### Livro (Book)

- **Attributes:**
  - `titulo`: string
  - `autor`: Autor

- **Methods:**
  - `__construct($titulo, $autor)`: Constructor to initialize a book with title and author.
  - `getTitulo()`: Returns the book's title.
  - `getAutor()`: Returns the book's author.

### Biblioteca (Library)

- **Attributes:**
  - `livros`: array

- **Methods:**
  - `adicionarLivro($livro)`: Adds a book to the library's books array.
  - `listarLivros()`: Returns an array with the books available in the library.

## Requirements

- PHP 7.4 or higher
- Web server (recommended: XAMPP)
