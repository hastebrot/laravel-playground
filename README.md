### Overview:

Laravel provides several starter kits.

- Laravel Installer (v4): https://github.com/laravel/installer
- Laravel Breeze (v1): https://github.com/laravel/breeze
- Laravel Jetstream (v2): https://github.com/laravel/jetstream
- Laravel UI (v3, legacy): https://github.com/laravel/ui

These starter kits contain different stacks.

- Laravel Install: Blade, Laravel Mix.
- Laravel Breeze: Blade, Laravel Mix, Tailwind CSS.
- Laravel Jetstream: Blade, Livewire, Laravel Mix, Tailwind CSS, Laravel Sanctum, Laravel Fortify.
- Laravel UI: Blade, Laravel Mix, Bootstrap CSS.

### Test Suites:

- Laravel Breeze: https://github.com/laravel/breeze/tree/1.x/stubs/default/tests
- Laravel Jetstream: https://github.com/laravel/jetstream/tree/2.x/tests
- Laravel UI: https://github.com/DCzajkowski/auth-tests

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
- Compile front-end assets with Laravel Mix using `npm install && npm run dev`.

### `laravel-breeze-app`

- Create Laravel app with `laravel new laravel-breeze-app`.
- Install Laravel Breeze with `composer require laravel/breeze --dev`.
- Scaffold Laravel Breeze with `php artisan breeze:install`.
- Compile front-end assets with Laravel Mix using `npm install && npm run dev`.

### `laravel-jetstream-app`

- Create Laravel app with `laravel new laravel-jetstream-app`.
- Install Laravel Jetstream with `composer require laravel/jetstream --dev`.
- Scaffold Laravel Jetstream with `php artisan jetstream:install livewire --teams`.
- Compile front-end assets with Laravel Mix using `npm install && npm run dev`.
- Publish Livewire stack's Blade components with `php artisan vendor:publish --tag=jetstream-views`.

### `laravel-ui-app`

- Create Laravel app with `laravel new laravel-ui-app`.
- Install Laravel UI with `composer require laravel/ui --dev`.
- Scaffold Laravel UI with `php artisan ui bootstrap --auth`.
- Compile front-end assets with Laravel Mix using `npm install && npm run dev`.

### `laravel-tailwind-app`

- Create Laravel app with `laravel new laravel-tailwind-app`.
- Install Laravel's front-end dependencies using `npm install`.
- Install Tailwind and its peer-dependencies: `npm install -D tailwindcss@latest postcss@latest autoprefixer@latest`.
- Create Tailwind configuration file: `npx tailwindcss init`.
- Configure Tailwind to remove unused styles in `tailwind.config.js`.
- Configure Tailwind with Laravel Mix in `webpack.mix.js`.
- Include Tailwind in application CSS in `resources/css/app.css`.
- Import stylesheet in application Blade layout in `resources/views/layouts/app.blade.php`.
