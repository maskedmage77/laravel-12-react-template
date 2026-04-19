# README

## Description

- Laravel 12 with Mantine.

## Installation

### Development 

#### Setup 

1. Copy the .env.example to .env and set the following variables
```
DB_PASSWORD=
DB_ROOT_PASSWORD=
```

2. Run the following command to start the development environment
```bash
docker compose -f docker-compose.dev.yml up --build -d
```

3. Shell into container
```
docker exec -it laravel-12-mantine-app sh
```

4. Install node packages
```
npm install
```

5. Generate Encryption Key
```
php artisan key:generate
```

6. Run migrations
```
php artisan migrate
```

#### Start the vite dev server

Shell into the container
```
docker exec -it laravel-12-mantine-app sh
```

Running vite dev server
```
npm run dev
```

### Production

```bash
docker compose -f docker-compose.prod.yml up --build -d

```
