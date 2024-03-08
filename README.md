# Bootcamp #01 Qualiters Club 
Criação de testes de API utilizando postman, newman e newman-htmlextra
Testes de API Rest do manual à CI/CD.

## O que é
Este repositório foi criado para o Bootcamp realizado sobre Testes de API Rest.

## Tecnologias utilizadas
- Postman 
- node version v20.10.0
- newman version 6.1.1
- newman-reporter-html

## Documentações
- Análise Técnica: Analise/
- Doc da API: [Consulte Swagger](https://serverest.dev/#/).
 
## Como instalar o ambiente
- Primeiro: Instalar o node na máquina [baixe aqui](https://nodejs.org/en).
- Segundo: Realize a instalação do newman de forma global [baixe aqui a dependencia](https://www.npmjs.com/package/newman).
```
npm install -g newman
```
- Terceiro: Faça a instalação da dependencia dos relatórios (opcional). [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html).
```
npm install -g newman-reporter-html
```

## Como rodar os testes

### Através do Postman Web ou Desktop.
- Importar a collection e o enviroment.
- Executar os testes de forma manual ou automatizado.

### Através do newman

- Utilize o console de sua preferência.
- Execute a seguinte llinha de comando para rodar os testes.
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute os testes com relatório.
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r htmlextra
```

### Report

Caso tenha escolhido por rodar os testes com o report htmlextra, foi gerado arquivo html com os resultados da massa de testes. Para analisar as validações, acesse a pasta **newman** que você criou no local em que os arquivos de collection e enviroment estão.

## Contato

email: omarkfrank@yahoo.com

linkedIn: https://www.linkedin.com/in/omarkfrank/
