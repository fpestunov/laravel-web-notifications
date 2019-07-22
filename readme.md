# Notifications with Laravel and Pusher

https://scotch.io/tutorials/create-web-notifications-using-laravel-and-pusher-channels

## Предустановка

- регистрируемся на pusher.com
- создаем приложение `laravel new laravel-web-notifications`
- добавляем pusher в наше приложение `composer require pusher/pusher-php-server`
- прописываем параметры приложения в `.env`:
```
PUSHER_APP_ID=
PUSHER_APP_KEY=
PUSHER_APP_SECRET=
```
- правим файл `config/broadcasting.php`:
```
'options' => [
  'cluster' => 'eu',
  'useTLS' => true
],
```
- в файле `config/app.php` раскоментировал `App\Providers\BroadcastServiceProvider::class`

Настройки завершены!

## Преступаем к разработке


