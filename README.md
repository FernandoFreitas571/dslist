# 🕹️ Projeto DSList - Intensivão Java Spring

[![NPM](https://img.shields.io/npm/l/react)](https://github.com/FernandoFreitas571/dslist/blob/main/LICENSE)

## 📚 Sobre o projeto

**DSList** é uma aplicação Java com Spring Boot que expõe uma API REST para manipulação de listas de jogos.

Os jogos podem ser organizados em listas (como "Favoritos", "Ação", "RPG", etc), e o sistema permite ordenar a posição dos jogos dentro dessas listas. O foco do projeto é praticar conceitos fundamentais de backend com Java, como:

- JPA/Hibernate  
- Relacionamentos muitos-para-muitos com atributos extras (via entidade associativa `Belonging`)  
- Criação de serviços RESTful  
- Estruturação de DTOs e camadas  

---

## 🧠 Modelo conceitual

Este é o modelo de dados usado na aplicação:

![Modelo Conceitual](https://github.com/FernandoFreitas571/dslist/blob/main/assets/modelo.png)

- `Game` representa os jogos disponíveis.  
- `GameList` representa uma lista de jogos (como playlists).  
- `Belonging` é a tabela intermediária que associa um jogo a uma lista, com a posição do jogo na lista.

---

## 🚀 Tecnologias utilizadas

### 🧩 Backend
- Java 11+
- Spring Boot
- Spring Data JPA
- Maven
- H2 Database (em memória)

---

## ⚙️ Como executar o projeto

### Pré-requisitos:
- Java 11 ou superior  
- Maven instalado

### Passos:

```bash
# Clonar o repositório
git clone https://github.com/FernandoFreitas571/dslist.git

# Entrar na pasta do projeto
cd dslist

# Executar o projeto com Maven
./mvnw spring-boot:run
````

A aplicação será executada por padrão na porta **8080**:

```
http://localhost:8080
```

Você pode testar os endpoints da API com ferramentas como **Postman** ou **Insomnia**.

---

## 📁 Estrutura de pastas (resumo)

```bash
src/
├── main/
│   ├── java/com/fernando/dslist/
│   │   ├── controllers/
│   │   ├── dto/
│   │   ├── entities/
│   │   ├── repositories/
│   │   └── services/
│   └── resources/
│       └── application.properties
```

---

## 📄 Licença

Este projeto está sob licença **MIT**.
Veja o arquivo [LICENSE](https://github.com/FernandoFreitas571/dslist/blob/main/LICENSE) para mais detalhes.

```

---

Pode colar isso direto no seu `README.md` no GitHub.  
Se quiser adicionar os **endpoints da API** também, posso montar uma seção extra com exemplos prontos!
```
