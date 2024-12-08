└── 3-tier
├── docker-compose.yml
├── mysql
│   ├── data
│   └── init.sql
├── nginx
│   ├── default.conf
│   └── index.html
└── php
├── Dockerfile
└── process_form.php

1. Create main directory as 3-tier       ---{mkdir 3-tier}
2. Inside 3-tier create 3 sub directory as nginx, php, mysql    ---{cd 3-tier}
3. write all the files as per directory name
4. create directory inside mysql named as data and leave it blank (when we will bind data directory it will work as a volume)
5. Open docker-compose file and check the all paths are correctly written in the file (check the spacing in file and manage it)
6. Then build the file and hit IP to browser      ---{docker-compose up -d}
