## Example of Laravel docker file.

### Installation:
Clone the repository
```sh
git clone https://github.com/siberfx/laravel9-docker.git
```
go into directory
```sh
cd laravel9-docker
```
Remove o versioning
```sh
rm -rf .git/
```
create your env file
```sh
cp .env.example .env
```
Change inside the env .env

![image](https://user-images.githubusercontent.com/61431715/157150667-9d6d49b7-9fe8-4a79-aae2-69441a966c43.png)
![image](https://user-images.githubusercontent.com/61431715/157150861-9fe29c50-1eaf-46ad-842b-95b61e1abf6b.png)
![image](https://user-images.githubusercontent.com/61431715/157150884-2ee002ea-fdf4-4d83-b406-475bb2ee7d41.png)


Build the container
```sh
docker-compose up -d
```
Accessing to php with bash
```sh
docker-compose exec app bash
```
Install dependencies
```sh
composer install
```
Generate application key inside .env
```sh
php artisan key:generate
```

Access: http://localhost:8080/
