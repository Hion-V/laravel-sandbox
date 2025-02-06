# Laravel-Sandbox

Dit is een project met als doel mezelf het web framework Laravel te leren door te experimenteren.

# Developing

Voer de volgende commandos uit om de ontwikkelomgeving op te zetten

```bash
git clone git@github.com:Hion-V/laravel-sandbox.git
cd laravel-sandbox
cp .env.example .env
```

Installeer composer dependencies

```bash
docker run --rm -v $(pwd)/app:/app composer install
```

Start stack en genereer key

```bash
docker compose up -d
docker compose exec app php artisan key:generate
```