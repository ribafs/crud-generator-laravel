# Gerador de CRUDs para laravel
Gerador de CRUDs para laravel com suporte a API

Gerador de CRUDs para Laravel

Com suporte ao laravel 9 e 10

https://github.com/sohelamin/crud-generator
```sh
composer require appzcoder/crud-generator --dev

php artisan vendor:publish --provider="Appzcoder\CrudGenerator\CrudGeneratorServiceProvider"
```
## Example de criação de CRUD
```sh
php artisan crud:generate Posts --fields='title#string; email#string;' --controller-namespace=App\\Http\\Controllers --form-helper=html
```
## Adicionar a rota em /routes/web.php:
```sh
Route::resource('/posts', 'App\Http\Controllers\PostsController');

php artisan route:clear

php artisan migrate

php artisan serve
```
http://127.0.0.1:8000/posts
`
## [Tutorial para API](api-tutorial.md) (in pt-br)
