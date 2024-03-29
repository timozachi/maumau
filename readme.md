# Laravel PHP Framework

[![Build Status](https://travis-ci.org/laravel/framework.svg)](https://travis-ci.org/laravel/framework)
[![Total Downloads](https://pos er.pugx.org/laravel/framework/d/total.svg)](https://packagist.org/packages/laravel/framework)
[![Latest Stable Version](https://poser.pugx.org/laravel/framework/v/stable.svg)](https://packagist.org/packages/laravel/framework)
[![Latest Unstable Version](https://poser.pugx.org/laravel/framework/v/unstable.svg)](https://packagist.org/packages/laravel/framework)
[![License](https://poser.pugx.org/laravel/framework/license.svg)](https://packagist.org/packages/laravel/framework)

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Laravel attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as authentication, routing, sessions, queueing, and caching.

Laravel is accessible, yet powerful, providing tools needed for large, robust applications. A superb inversion of control container, expressive migration system, and tightly integrated unit testing support give you the tools you need to build any application with which you are tasked.
z
## Official Documentation

Documentation for the framework can be found on the [Laravel website](http://laravel.com/docs).

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](http://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell at taylor@laravel.com. All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).

#INSTRUÇÕES DE INSTALAÇÃO

Passos (Obs: isto assume que você tem php e mysql,):
1. composer install
2. cp .env.example .env
3. Edite o .env como necessário
4. Crie o banco com o seguinte SQL: CREATE DATABASE maumau DEFAULT CHARACTER SET utf8 COLLATE utf8_unicode_ci;
5. php artisan key:generate
6. php artisan migrate --seed
7. Execute o arquivo de sql "maumau_data.sql" na pasta database para popular o banco com cartas e modalidades
8. Crie o virtual host (seja nginx ou apache) que aponte para a pasta pública, com o domain de sua preferência (eu uso "maumau.local")
9. Para iniciar o servidor de WebSocket execute: php artisan server:init
10. Você pode acessar o painel de administração no endereço: http://maumau.local/admin/, com o usuário "admin@email.com" e senha "123456"
11. Você pode acessar o jogo pelo endereço: http://maumau.local/jogar