# Cities

Cadastro simples de cidades para exercitar alguns tópicos do livro "ASP.NET Core 8 and Angular" de Valerio de Sanctis.

## Backend

O backend é uma aplicação .NET 8 Web API e foi configurada com os comandos abaixo:

1. Criação da aplicação:

```bash
dotnet new webapi -n backend -controllers
```

O parâmetro `-controllers` é para que não seja criada uma minimal API.

2. Geração do arquivo `.gitignore` (já na pasta do backend):

```bash
dotnet new gitignore
```

3. Edição do arquivo `Properties\launchSettings.json`:

-   Todas as propriedades `launchBrowser` foram alteradas para `false`;
-   Todas as portas de HTTP e HTTPS foram alteradas para `40080` e `40443`, respectivamente.

## Frontend

O frontend é uma aplicação Angular 17 e foi configurada com os comandos abaixo:

1. Criação da aplicação (com parâmetros padrão):

```bash
ng new frontend
```

2. Adição do Angular Material (com parâmetros padrão):

```bash
ng add @angular/material
```

3. Configuração dos arquivos de `environment`:

-   Criação:

```bash
ng generate environments
```

-   Adicionadas URLs da API no arquivo `environment.ts`.

4. Migrado `css` para `scss` com o assistente abaixo:

```bash
ng add schematics-scss-migrate
```
