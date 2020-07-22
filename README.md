# Operações Bancárias via API RestFull

Aplicação para disponibilizar via API RestFull informações sobre saldo em conta de usuários desenvolvido no bootcamp fullstack da IGTI.

## <img src="https://img.icons8.com/ios-filled/20/000000/browser-window.png"/> Insomnia

<p align="center">
  <img src="https://github.com/cicerorod/igti-fullstack-mod2-my-bank-api/blob/master/img/tela.PNG">
</p>

## ![](https://img.icons8.com/metro/20/000000/run-command.png) Execução

1. Clonar via prompt de comando o projeto em uma pasta de sua preferência: `git clone https://github.com/cicerorod/igti-fullstack-mod2-my-bank-api.git`
2. Acessar a pasta principal do projeto via prompt de comando.  Ex: `cd igti-fullstack-mod2-my-bank-api`;
3. Executar o comando `yarn` para baixar as dependências. Ex: `yarn`;
4. Executar o comando `yarn start`. Ex: `yarn start`
5. Acessar o endereço `http://localhost:4000/account` conforme rotas definidos no item rotas

### ![](https://img.icons8.com/metro/20/000000/run-command.png) Rotas

#### `/account/`

HTTP GET solicitação que retorna uma resposta JSON contendo as contas cadastradas.

##### `GET`: `http://localhost:4000/account/`

##### Exemplo de retorno:

```json
{
  "accounts": [
    {
      "id": 2,
      "name": "Cícero Rodrigues",
      "balance": 10
    },
    {
      "id": 3,
      "name": "Maria das Dores",
      "balance": 10
    }
  ]
}
```

#### `/account/`

HTTP POST para inserção de registros.

##### `Post`: `http://localhost:4000/account/`

##### Exemplo de parâmetro:

```json
{
  "name": "João da Silva",
  "balance": 10.0
}
```

##### Exemplo de retorno:

```Json

{
      "id": 4,
      "name": "João da Silva",
      "balance": 10
}

```

#### `/account/id`

HTTP GET solicitação que retorna um JSON contendo as informações do `id` pesquisado.

##### `GET`: `http://localhost:4000/account/id`

##### Exemplo: `http://localhost:4000/account/2`

##### Exemplo de retorno:

```json
{
  "id": 2,
  "name": "Cícero Rodrigues",
  "balance": 10
}
```

#### `/account/`

HTTP PUT, solicitação que atualiza as informações de contas.

##### `PUT`: `http://localhost:4000/account/`

##### Exemplo de parâmetro:

```json
{
  "id": 4,
  "name": "João da Silva",
  "balance": 100
}
```

##### Exemplo de retorno:

```Json

{
      "id": 4,
      "name": "João da Silva",
      "balance": 100
}

```

#### `/grade/id`

HTTP DEL, solicitação para excluir um registro referente ao `id`.

##### `DEL`: `http://localhost:4000/account/id`

##### Exemplo: `http://localhost:4000/account/1`

##### Exemplo de retorno:

```Request

200OK

```

#### `/account/transacao`

HTTP POST para atualização do saldo em conta..

##### `Post`: `http://localhost:4000/account/transacao`

##### Exemplo de parâmetro:

```json
{
  "id": 2,
  "value": 100
}
```

##### Exemplo de retorno:

```Json
{
  "id": 2,
  "name": "Cícero Rodrigues",
  "balance": 110
}

```

<!-- :hammer:-->

## ![](https://img.icons8.com/ios-filled/20/000000/hammer.png) Recursos utilizados:

- **[NodeJS](https://nodejs.org/en/)**
- **[winston]()**
- **[nodemon]()**
- **[Json](https://www.w3schools.com/js/js_json_intro.asp)**
- **[Express](http://expressjs.com/)**
- **[Insomnia](https://insomnia.rest/download/)**
- **[Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=hackingcarreira_wmc-github-gllemos)**

## ![](https://img.icons8.com/ios-glyphs/20/000000/pull-request.png) Contribuições

1. Faça o _fork_ do projeto (<https://github.com/cicerorod/igti-fullstack-mod2-my-bank-api/fork>)
2. Crie uma _branch_ para sua modificação (`git checkout -b feature/[nome]`)
3. Faça o _commit_ (`git commit -am 'Add files [nome]'`)
4. _Push_ (`git push origin feature/[nome]`)
5. Crie um novo _Pull Request_

## ![](https://img.icons8.com/ios-glyphs/22/000000/code-file.png) Desenvolvedor

<img src="https://avatars.githubusercontent.com/cicerorod" width=115>

[![](https://img.icons8.com/fluent/30/000000/github.png)](https://github.com/cicerorod)
[![](https://img.icons8.com/metro/25/000000/linkedin.png)](https://www.linkedin.com/in/c%C3%ADcero-rodrigues-89623784/)
[![](https://img.icons8.com/metro/25/000000/facebook.png)](https://www.facebook.com/cicero.rodrigues.90834)
[![](https://img.icons8.com/material-rounded/29/000000/instagram-new.png)](https://www.instagram.com/cicero_rod/)
[![](https://img.icons8.com/metro/26/000000/email.png)](mailto:cicerorod@gmail.com)

<p align="center">
  <img src="https://img.icons8.com/wired/32/000000/icons8-new-logo.png" >
  </br>
  <a href="https://icons8.com/icon/">Icons by Icons8</a>
  
</p>
