# School-Api
Projeto de escola para a disciplina de POS (Programação Orientada a Serviços)

# Como executar
> Passos para executar o projeto

## Dependências
Primeiramente, é necessário utilizar/instalar as dependências do projeto listadas abaixo.

* [Composer](https://getcomposer.org)
* [Laravel](https://laravel.com)

## Definir porta
Para definir uma porta específica execute o comando `php artisan serve --port=8888`

## Requisições GET
**Requisições** | **Retorno** | **Descrição**
--- | --- | ---
`/` | *{“hello_url” : “/hello”}* | Fornecimento de todos os padrões de URL
`/hello` | *Hello, World!* | URL de teste

---
# Código
> Home
```php
Route::get('/', function () {
    return '{“hello_url” : “/hello”}';
});
```
> Hello
```php
Route::get('/hello', function () {
    return 'Hello, World!';
});
```
---
