Esse repositório faz parte do curso de formação em DevOps realizado pela Alura e tem por objetivo a prática de Git e GitHub.

# AllBooks 📖📚

Projeto de loja virtual disponibilizado pela Alura para prática de Git e GitHub, abordando os seguintes conteúdos:

- Conhecer os principais comandos de trabalho no GitHub
- Absorver conhecimentos em GitFlow e GitHub Actions
- Aprender a lidar com commits, conflitos, issues e PRs
- Organizar fluxos e projetos com GitHub Actions
- Trabalhar com segurança e Dependabot
  
# JSONServer + JWT Auth

Essa é uma API Rest mockada, utilizando json-server e JWT.

## 🛠️ Instalação

```bash
$ npm install
$ npm run start-auth
```
## 🛠️ Como se registrar?

Você pode fazer isso efetuando uma requisição post para:

```
POST http://localhost:8000/public/registrar
```

Você pode utilizar os seguintes dados:


```
{
    "nome": "vinicios neves",
    "email": "vinicios@alura.com.br",
    "senha": "123456",
    "endereco": "Rua Vergueiro, 3185",
    "complemento": "Vila Mariana",
    "cep": "04101-300"
}
```

Observe que o e-mail é um campo único e usuários com e-mails duplicados não serão persistidos.

## 🛠️ Como fazer login?

Você pode fazer isso efetuando uma requisição post para:

```
POST http://localhost:8000/public/login
```

Com os seguintes dados:


```
{
  "email": "vinicios@alura.com.br",
  "senha":"123456"
}
```

Você vai receber um token no seguinte formato:

```
{
   "access_token": "<ACCESS_TOKEN>",
   "user": { ... dados do usuário ... }
}
```

## Autenticar próximas requests?

E então, adicionar este mesmo token ao header das próximas requisições:

```
Authorization: Bearer <ACCESS_TOKEN>
```

