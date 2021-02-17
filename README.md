# Ark IDs Resolver

## Introduction 

This repository is separated from the Ark Services(https://github.com/digitalutsc/ark-services), and it will be Ark ID lookup for upcoming traffic and the landing page. With this, the back-end operations interface will be placed behind the VPN for security measures. 

## Installation

1. Create a site in `/etc/apache2/sites-available` and point it to this repo.
2. Filled out the Mysql database credentails at `config/MysqlArkConf.php` to have the resolver connected to exsiting Ark IDs database. 

````php 
<?php

namespace Ark\Resolver\Library;

class MysqlArkConf
{
    static public $mysql_host = '';
    static public $mysql_user = '';
    static public $mysql_passwd = '';
    static public $mysql_dbname = '';
    static public $mysql_port = 3306;
}


