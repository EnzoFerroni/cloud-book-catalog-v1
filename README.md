# Projeto01 Nuvem v1

[![Java](https://img.shields.io/badge/Java-Spring%20Boot-6DB33F?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Next.js](https://img.shields.io/badge/Next.js-14-000000?logo=nextdotjs)](https://nextjs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

First iteration of a book catalog for a cloud services course: a Spring Boot API and a Next.js front end, each in its own container.

> This is an early prototype. The finished, deployable version is
> [Projeto01-Biblioteca-AWS](https://github.com/EnzoFerroni/Projeto01-Biblioteca-AWS).

## Table of Contents

- [About](#about)
- [Architecture](#architecture)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [License](#license)

## About

Built for the cloud services course at Universidade Presbiteriana Mackenzie (2024).
This version explored the stack before the final delivery: a Spring Boot service with
a `Book` entity (title, author, description, cover) and a Next.js page that renders
the books as cards.

## Architecture

| Service | Stack | Port |
| --- | --- | --- |
| `back` | Spring Boot REST API, `GET /books` | 25000 |
| `front` | Next.js 14 (App Router, TypeScript) | 3000 |

## Getting Started

Requirements: JDK 17+, Maven and Node.js 18+.

```bash
git clone https://github.com/EnzoFerroni/Projeto01-Nuvemv1.git
cd Projeto01-Nuvemv1

cd "back/Projeto Final/minhaBiblioteca"
./mvnw spring-boot:run

cd ../../../front/serv-nuvem-proj
npm install
npm run dev
```

## Project Structure

```
├── back/Projeto Final/minhaBiblioteca/   Spring Boot API and Dockerfile
└── front/serv-nuvem-proj/                Next.js app (page, BookCard component)
```

## License

Released under the [MIT License](LICENSE). Copyright (c) 2024 Enzo Ferroni.
