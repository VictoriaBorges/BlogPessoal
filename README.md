# Blog Pessoal

## 📌 Sobre o Projeto
O **Blog Pessoal** é uma aplicação web desenvolvida em Java utilizando Spring Boot. O objetivo do projeto é permitir que usuários criem, editem e visualizem postagens em um blog pessoal. A aplicação é estruturada com boas práticas de desenvolvimento e pode ser utilizada como base para estudos de APIs REST.

## 🚀 Tecnologias Utilizadas
- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **MySQL**
- **Docker**
- **Maven**

## 📂 Estrutura do Projeto
```
BlogPessoal/
├── src/
│   ├── main/
│   │   ├── java/com/seuusuario/blogpessoal/
│   │   │   ├── controller/
│   │   │   ├── model/
│   │   │   ├── repository/
│   │   │   ├── service/
│   ├── resources/
│   │   ├── application.properties
├── .gitignore
├── Dockerfile
├── pom.xml
└── README.md
```

## ⚙️ Configuração e Execução

### Pré-requisitos
Antes de iniciar, verifique se você possui os seguintes requisitos instalados:
- Java 17 ou superior
- Maven
- MySQL
- Docker (opcional para containerização)

### Configuração do Banco de Dados
1. Crie um banco de dados MySQL:
   ```sql
   CREATE DATABASE blog_pessoal;
   ```
2. Configure o arquivo `application.properties` com as credenciais do seu banco de dados:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/blog_pessoal
   spring.datasource.username=root
   spring.datasource.password=senha
   spring.jpa.hibernate.ddl-auto=update
   ```

### Executando a Aplicação
1. Clone o repositório:
   ```bash
   git clone https://github.com/VictoriaBorges/BlogPessoal.git
   ```
2. Acesse o diretório do projeto:
   ```bash
   cd BlogPessoal
   ```
3. Compile e execute o projeto com Maven:
   ```bash
   mvn spring-boot:run
   ```

### Executando com Docker (Opcional)
Se desejar rodar a aplicação em um container Docker, execute:
```bash
docker build -t blog-pessoal .
docker run -p 8080:8080 blog-pessoal
```

## 🛠️ Endpoints da API
A aplicação expõe uma API REST. Alguns dos principais endpoints são:

- `GET /postagens` → Retorna todas as postagens
- `POST /postagens` → Cria uma nova postagem
- `PUT /postagens/{id}` → Atualiza uma postagem existente
- `DELETE /postagens/{id}` → Exclui uma postagem

## 📌 Contribuição
Fique à vontade para contribuir com o projeto! Para isso:
1. Faça um fork do repositório
2. Crie uma branch para sua feature (`git checkout -b minha-feature`)
3. Faça commit das suas alterações (`git commit -m 'Adicionando nova feature'`)
4. Faça push para a branch (`git push origin minha-feature`)
5. Abra um Pull Request

## 📄 Licença
Este projeto está sob a licença MIT. Sinta-se livre para usá-lo e modificá-lo conforme necessário!

---
Desenvolvido por [Victoria Borges](https://github.com/VictoriaBorges) 🚀

