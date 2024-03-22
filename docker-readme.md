Make any changes to the docker-compose.yml file that you want such as the database name, user, and password. Then run the following commands.
launch the docker containers:

```bash
docker-compose up -d
```

set file permissions for sftp:
```bash
docker ps
docker exec -it docker-wordpress_wordpress_1 bash
chmod -R go+w /var/www/html/wp-content
```

You can access the wordpress site at http://localhost:8000

You can log into phpMyAdmin at http://localhost:8081

You can use filezilla to connect to the server using sftp and port 2222