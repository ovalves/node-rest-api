# Introdução
Uma API simples feita com nodejs.

## API
### Instalação
Para rodar a API localmente, siga as instruções abaixo:

1. Faça o fork [deste repositório](https://github.com/ovalves/simple-node-api) e crie o seu projeto a partir dele
2. Clone seu próprio repositório
3. Inicie a instalação das dependências do projeto excutando `npm install`
    - Caso seja necessário, execute: `npm audit fix` _(o próprio npm irá te instruir a fazer isso)_
4. Se precisar alterar as informações padrões do servidor, copie o arquivo **.env.example** para **.env** e altere seus valores
    - O endereço padrão é: `http://localhost:3000`
5. Execute o comando `npm run serve` para rodar o servidor

### Uso
1. Busque um access token através do endpoint `GET /auth/login` informando o email e senha do usuário
    - Eles estão localizados em [src/Database/data/users.json](https://github.com/ovalves/simple-node-api/blob/main/src/Database/data/users.json)
2. Utilize o token em todas as requisições seguintes através do cabeçalho `Authorization: Bearer <TOKEN>`

### Endpoints
- `GET /users`
- `GET /posts`
- `POST /posts`
- `DELETE /posts/<id>`
- `GET /categories`
