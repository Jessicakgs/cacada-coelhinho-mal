# 🐰 Caçada ao Coelhinho do Mal - API REST com Spring Boot

Um jogo de mistério e investigação... onde o objetivo é encontrar o **Coelhinho do Mal**, o grande vilão da Páscoa! 😈🥚  
Construa suas tentativas com lógica e atenção às pistas para capturar o coelho antes que ele roube todos os ovos!

---

## 🎯 Objetivo do Projeto

Este projeto foi criado com o propósito de estudo e aprimoramento em desenvolvimento de APIs REST usando **Java com Spring Boot**.  
É um projeto de nível **intermediário**, com regras de negócio, pontuação, persistência de dados e ranking de jogadores.

---

## 🧩 Como funciona o jogo?

1. O jogador se cadastra com um **nickname**
2. Ele recebe:
   - Uma **lista de códigos** (chaves secretas)
   - Uma **lista de locais suspeitos**
3. Ele escolhe um **local** e acessa uma **pista**
4. Com base na pista, ele tenta um **código**
5. A cada tentativa:
   - Se acertar o código mas o coelho **não estiver lá**, ganha pontos
   - Se errar o código, perde pontos
   - Se acertar o código **e** for o local do coelho, **vence o jogo!**
6. Ao final, o jogador aparece no **ranking** com sua pontuação

---

## 🔧 Tecnologias Utilizadas

- Java 21+
- Spring Boot
- Spring Web
- Spring Data JPA
- Docker
- MapStruct 
- Swagger (para documentação da API)
- JUnit/Testes 

---

## 📁 Estrutura Inicial da API

| Recurso | Endpoint |
|--------|----------|
| Cadastrar Jogador | `POST /players` |
| Listar Códigos | `GET /codes` |
| Listar Locais Suspeitos | `GET /locations` |
| Obter Pista de um Local | `GET /locations/{id}/hint` |
| Tentar Capturar o Coelho | `POST /hunt` |
| Ver Ranking | `GET /ranking` |

---

## 🧠 Conceitos Envolvidos

- Regras de negócio com lógica de jogo
- Respostas diferentes conforme ação do jogador
- Modelagem relacional de entidades
- Sistema de pontuação e ranking
- Lógica condicional baseada em tentativas

---

## 🚀 Como Rodar o Projeto (em breve)

```bash
# clone o projeto
git clone https://github.com/Jessicakgs/cacada-coelhinho-mal.git

# entre na pasta
cd cacada-coelhinho-mal

# rode o projeto (via sua IDE ou usando o Maven/Gradle)
