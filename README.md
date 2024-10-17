# ServeRestAPI
Criação de testes de API utilizando Postman, Newman e Newman-htmlextra

## Tecnologias utilizadas
- Postman Web
- node version v20.16.0
- newman v6.2.1
- newman-reporter-html

## Documentação
Doc da API: [Consulte Swagger]([https://serverest.dev/)

## Como instalar o ambiente
Primeiro: instale o node em seu computador [baixe aqui](https://nodejs.org/en/download)

Segundo: realize a instalação do newman de forma global [baixe aqui a dependencia](https://www.npmjs.com/package/newman)
ou por comando no terminal [newman html] (npm install -g newman-reporter-html)

Terceiro: realize a instalação da dependencia dos relatórios, basta colocar os seguintes comandos no terminal:
[newman htmlextra](npm install -g newman-reporter-htmlextra)
[newmancli](npm install -g newman)

## Como rodar os testes

### Pelo Postman web ou desktop
- Importe a collection e o environment
- Execute os testes de forma manual ou automatizada

### Pelo newman 
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
```
newman run .\ServeRest.postman_collection.json -e .\ServeRest_env.postman_environment.json -r htmlextra
```
- Execute os testes com relatório
```
newman run .\ServeRest.postman_collection.json -e .\ServeRest_env.postman_environment.json -r htmlextra
```

### Report
Se você optou por rodar o teste com report htmlextra, você gerou um arquivo html com o resultado dos teses e para verificar as validações você pode abrir a pasta **newman** que foi criada no local em que os arquivos collection e environment se encontram.

## Entre em contato
Email: kayque.rocha96@outlook.com

Linkedin:https://www.linkedin.com/in/kayque-rocha-001585324/
