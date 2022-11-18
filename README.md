# Mars Rover Challenge - Teste Emana Group 


![exemplo imagem](https://media-exp1.licdn.com/dms/image/D4D0BAQHB4UiiPJpO2A/company-logo_100_100/0/1664893430143?e=1677110400&v=beta&t=8ULE0gmaHsgRkmCCzN_ZhSCmuLh7Ot_-mcCcMPFDHBo)

> ## Backend em NodeJS, Javascript, ExpressJS, PostgresSQL, Sequelize
> ## Frontend em ReactJS.

A squad of robotic rovers are to be landed by NASA on a plateau on Mars.

This plateau, which is curiously rectangular, must be navigated by the rovers so that their on-board cameras can get a complete view of the surrounding terrain to send back to Earth.

A rover’s position and location is represented by a combination of x and y co-ordinates and a letter representing one of the four cardinal compass points. The plateau is divided up into a grid to simplify navigation. An example position might be 0, 0, N, which means the rover is in the bottom left corner and facing North.

In order to control a rover , NASA sends a simple string of letters. The possible letters are ‘L’, ‘R’ and ‘M’. ‘L’ and ‘R’ makes the rover spin 90 degrees left or right respectively, without moving from its current spot. ‘M’ means move forward one grid point, and maintain the same heading.

Assume that the square directly North from (x, y) is (x, y + 1).

## ✅ Funcionalidades
- Realizar o deploy desses rovers, bem como as validações de regras, através do Frontend criado especificamente para consumir essa API desenvolvida.
- Salvar os registros dos deploys dos rovers na base de dados PostgresSQL. 
- Listar o resultados dos deploys através de um Report que pode ser executado direto do Frontend.

## ✅ Endpoints
* POST /rover
* GET /rover

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

* Ter o Docker instalado (preferência mais atualizado) e rodando para que seja criada a base de dados dessa aplicação. (Procurar fechar todos os serviços e containeres que já estiverem rodando para evitar conflito de portas)

* NodeJS Instalado na máquina.

## 🚀 Instalação

Para instalação e funcionamento, siga estas etapas:

### Clonar Projeto
```
git clone https://github.com/saviopinho/emana-teste-fullstack.git
```

## Configurar Variáveis de Ambiete
O arquivo .env já está preenchido com os dados necessários para o funcionamento padrão.

### Acessar raiz do projeto
```
cd emana-teste-fullstack
```

### Acessar raiz do Backend
```
cd backend
```

### Instalar Packages do Backend
```
npm install
```

### Criar e subir container PostgresSQL com Docker
```
npm run docker:compose:down

npm run docker:compose:up
```

### Executar a migration da tabela de backlog
```
npm run migration:run
```

### Iniciar nosso servidor API 
* Caso queira rodar o servidor e testar manualmente
```
npm run start
```
* Caso queria rodar os testes de integração
```
npm run test
```

## ☕ Observações

* Em caso de conflito de portas ao executar o comando docker compose, realizar todo o processo do início, porém alterando o .env para as portas que estarão disponíveis
* Usar a ferramenta de sua preferência para testar as rotas e os endpoints criados
