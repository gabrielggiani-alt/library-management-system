# biblioteca-java

A library management system in Java with full CRUD on four modules (Author, Book, User, Loan) and an interactive CLI menu.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)

---

## About

- Package layout: `modelo/` (domain), `controle/` (CRUD controllers), `MainBiblioteca` (CLI entry point)
- Abstract superclass `Pessoa` extended by `Autor` and `Usuario` (inheritance + abstraction)
- Polymorphic `exibirInfo()` overridden in each subclass
- In-memory storage with `ArrayList` and a borrow/return business rule that updates book availability
- Includes a slide deck (`Apresentacao_Biblioteca.pdf`)

## Running

Open in NetBeans (`build.xml` + `nbproject/` are set up for it), or compile directly:

```bash
javac -d out src/ucb/poo/biblioteca/**/*.java src/ucb/poo/biblioteca/MainBiblioteca.java
java -cp out ucb.poo.biblioteca.MainBiblioteca
```

**Author:** Gabriel Gomes Giani
