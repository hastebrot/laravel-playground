### Overview:

Laravel provides several starter kits with different stacks.

- Laravel Installer (v4): https://github.com/laravel/installer
- Laravel Breeze (v1): https://github.com/laravel/breeze
- Laravel Jetstream (v2): https://github.com/laravel/jetstream
- Laravel UI (v3, legacy): https://github.com/laravel/ui

### Preparation:

- Install `php` command and `compose` dependency manager.
- Add `~/.composer/vendor/bin` to your `PATH`.
- Install Laravel installer with `composer global require laravel/installer`.

~~~
$ laravel --version
Laravel Installer 4.2.4
~~~

### `laravel-app`

- Create Laravel app with `laravel new laravel-app`.

### `laravel-breeze-app`

- Create Laravel app with `laravel new laravel-breeze-app`.
- Install Laravel Breeze with `composer require laravel/breeze --dev`.
- Scaffold Laravel Breeze with `php artisan breeze:install`.

### `laravel-jetstream-app`

- Create Laravel app with `laravel new laravel-jetstream-app`.
- Install Laravel Jetstream with `composer require laravel/jetstream --dev`.
- Scaffold Laravel Jetstream with `php artisan jetstream:install livewire --teams`.

### `laravel-ui-app`

- Create Laravel app with `laravel new laravel-ui-app`.
- Install Laravel UI with `composer require laravel/ui --dev`.
- Scaffold Laravel UI with `php artisan ui bootstrap --auth`.
- Compile fresh scaffolding with `npm install && npm run dev`.
