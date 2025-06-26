# Desafio Validação e Segurança

Este projeto é parte de um desafio prático com foco em **validação de dados**, **controle de acesso** e **segurança** em uma API REST desenvolvida com Java e Spring Boot.

## 🎯 Objetivo

Implementar as funcionalidades necessárias para que **todos os testes automatizados** do projeto base sejam aprovados.

O projeto simula um sistema de **eventos** e **cidades**, com uma relação N-1 (vários eventos para uma cidade).

---

## 🔐 Regras de Controle de Acesso

- ✅ **Públicas (sem login):**
  - `GET /events`
  - `GET /cities`

- 🔐 **Acesso permitido para perfis CLIENT e ADMIN:**
  - `POST /events`

- 🔐 **Acesso exclusivo para perfil ADMIN:**
  - Todos os outros endpoints.

---

## ✅ Regras de Validação

### Cidade (City)

- `name`: **não pode ser vazio**

### Evento (Event)

- `name`: **não pode ser vazio**
- `date`: **não pode ser no passado**
- `city`: **não pode ser nula**

---

## 🛠️ Tecnologias e Conceitos

- **Java 17+**
- **Spring Boot**
- **Spring Security + OAuth2**
- **Bean Validation (javax.validation)**
- **Spring Data JPA**
- **TDD com JUnit e MockMvc**

---

## 📋 Competências Avaliadas

- Desenvolvimento de API REST com **TDD** (Test-Driven Development)
- Implementação de segurança com **Spring Security** e **OAuth2**
- **Controle de acesso** baseado em **rotas** e **perfis de usuário**
- Validação de dados com **Bean Validation**

---