### Docker
#### Go to the docker container
    ```
    docker-compose ps
    ```
    or
    ```
    docker-compose ps -a
    ```

    *Collect The Docker Container Name*
    ```
    docker exec -it <containerName> bash
    ```

    Example:
    ```
    docker exec -it gsbd_php-fpm_1 bash
    ```

#### Permission Problem?
##### User Permission - If permission problem
###### Laravel installed in current folder, just change your current folder to you installation folderr
```
chown -R www-data:www-data /var/www/laravel/current
```
```
chmod -R 775 /var/www/laravel/current/storage
```