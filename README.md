# 3-Tier Architecture with Docker

This task demonstrates a simple 3-tier architecture using Docker. It includes three main services:

1. **MySQL** - The database layer for storing data.
2. **PHP** - The application layer that processes the logic and communicates with the database.
3. **Nginx** - The presentation layer, which serves static content and proxies PHP requests.

## Project Structure

```plaintext
3-tier
├── docker-compose.yml        
├── mysql
│   ├── data                 
│   └── init.sql              
├── nginx
│   ├── default.conf          
│   └── index.html          
└── php
    ├── Dockerfile            
    └── handler.php      

```
1. Create main directory as 3-tier.       ---{mkdir 3-tier}
2. Inside 3-tier create 3 sub directory as nginx, php, mysql.    ---{cd 3-tier}
3. Write all the files as per directory name show above.
4. Create directory inside mysql named as data and leave it blank. (when we will bind data directory it will work as a volume)
5. Open docker-compose file and check the all paths are correctly written in the file. (check the spacing in file and manage it)
6. Then run the docker-compose file  ---{docker-compose up -d} and,
7. Hit the IP on the browser.     
