# API de Gerenciamento de Tarefas

Este projeto foi desenvolvido como atividade da disciplina de **Desenvolvimento Web Backend** da UNINTER.  
O objetivo é implementar uma API RESTful para gerenciamento de tarefas utilizando **Java + Spring Boot + MySQL**.

---

## 🚀 Tecnologias Utilizadas
- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- MySQL
- Postman (para testes e documentação)

---

## 📌 Funcionalidades da API

- **Criar uma tarefa**
  - `POST /tarefas`
  - Exemplo de JSON:
    ```json
    {
    "nome": "Testes unitários e integração",
    "dataEntrega": "2025-12-20",
    "responsavel": "Camila Rodrigues"
    }
    ```

- **Listar todas as tarefas**
  - `GET /tarefas`

- **Buscar uma tarefa por ID**
  - `GET /tarefas/{id}`

- **Atualizar uma tarefa**
  - `PUT /tarefas/{id}`

- **Deletar uma tarefa**
  - `DELETE /tarefas/{id}`

---

## 🗄️ Estrutura do Projeto
- `model/` → Contém a entidade **Tarefa**
- `repository/` → Interface **TarefaRepository**
- `controller/` → Classe **TarefaController** com os endpoints REST

---

## ⚙️ Configuração do Banco de Dados
No arquivo `application.properties` configure o acesso ao seu MySQL:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/tarefas_db
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
```

## 👩‍🎓 Autora
Juliana Rodrigues de Souza
