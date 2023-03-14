## SET ENVIROMENT

1. `$ composer install`
2. `$ npm install`
3. Renombrar fichero .env.example a .env y crear base de datos
4. `$ php artisan migrate`

## crear key para aplicación
`$ php artisan key:generate`

## Insertar Roles en la tabla de roles
`INSERT INTO `roles` (`id`, `nombre`) VALUES ('1', 'Administrador'), ('2', 'Empleado');`
## Insertar Niveles
`INSERT INTO `niveles` (`id`, `nombre`) VALUES ('1', 'Administrador'), ('2', 'Empleado');`



## SET ADMIN USER
`INSERT INTO `users` (`id`, `name`, `apellidos`, `email`, `password`, `alias`, `rol_id`, `direccion`, `cp`, `ciudad`, `provincia`, `pais`, `movil`, `telefono`, `avatar`, `nif`, `iban`, `fecha_nacimiento`, `nivel_id`, `puesto_id`, `otros`, `remember_token`, `created_at`, `updated_at`, `last_login`, `sueldo`, `precio_hora`, `active`) VALUES (NULL, 'admin', 'admin', 'admin@mail.com', '$2a$10$m3nEMvygNO0vX.JRvYtLnuzevpaQ61KJBLcc8rG0FsqTRGsklt8Nm', 'admin', '1', 'UTN', '57000', 'Nezahualcoyotl', 'Neza', 'Mexico', '1234567890', '0987654321', '', '0125849', '1345687', '2000-03-12 00:00:00', '1', '1', '', NULL, '0000-00-00 00:00:00.000000', '0000-00-00 00:00:00.000000', NULL, NULL, NULL, '1');`
`$ $password= admin`
`$ $ingreso de pass base de datos= $2a$10$m3nEMvygNO0vX.JRvYtLnuzevpaQ61KJBLcc8rG0FsqTRGsklt8Nm `
# SET USER EMPLEADO
`INSERT INTO `users` (`id`, `name`, `apellidos`, `email`, `password`, `alias`, `rol_id`, `direccion`, `cp`, `ciudad`, `provincia`, `pais`, `movil`, `telefono`, `avatar`, `nif`, `iban`, `fecha_nacimiento`, `nivel_id`, `puesto_id`, `otros`, `remember_token`, `created_at`, `updated_at`, `last_login`, `sueldo`, `precio_hora`, `active`) VALUES (NULL, 'empleado', 'empleado', 'empleado@mail.com', '$2a$12$F3EjJMpuCbnpFGcu0WsR0uCKjdcs/M3ZRBFKY7iHDytl.ZTgvMwEm', 'empleado', '2', 'UTN', '57000', 'Nezahualcoyotl', 'Neza', 'Mexico', '1234567890', '0987654321', '', '0125849', '1345687', '2000-03-12 00:00:00', '2', '2', '', NULL, '0000-00-00 00:00:00.000000', '0000-00-00 00:00:00.000000', NULL, NULL, NULL, '1');`
`$ $password= empleado`
`$ $ingreso de pass base de datos= $2a$12$F3EjJMpuCbnpFGcu0WsR0uCKjdcs/M3ZRBFKY7iHDytl.ZTgvMwEm `

## LUNCH
`$ php artisan serve`

##ASSETS
 Debe almacenarse en resources mediante js y sass y luego compilarse con gulp - elixir (ver gulpfile.js)

 De momento la mayoría de las cosas estan en public directamente


## Laravel PHP Framework

[![Build Status](https://travis-ci.org/laravel/framework.svg)](https://travis-ci.org/laravel/framework)
[![Total Downloads](https://poser.pugx.org/laravel/framework/d/total.svg)](https://packagist.org/packages/laravel/framework)
[![Latest Stable Version](https://poser.pugx.org/laravel/framework/v/stable.svg)](https://packagist.org/packages/laravel/framework)
[![Latest Unstable Version](https://poser.pugx.org/laravel/framework/v/unstable.svg)](https://packagist.org/packages/laravel/framework)
[![License](https://poser.pugx.org/laravel/framework/license.svg)](https://packagist.org/packages/laravel/framework)

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Laravel attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as authentication, routing, sessions, queueing, and caching.

Laravel is accessible, yet powerful, providing powerful tools needed for large, robust applications. A superb inversion of control container, expressive migration system, and tightly integrated unit testing support give you the tools you need to build any application with which you are tasked.

## Official Documentation

Documentation for the framework can be found on the [Laravel website](http://laravel.com/docs).

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](http://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell at taylor@laravel.com. All security vulnerabilities will be promptly addressed.

### License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)
