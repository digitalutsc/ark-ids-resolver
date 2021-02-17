# Ark IDs Resolver

## Introduction 

This repository is separated from the Ark Services(https://github.com/digitalutsc/ark-services), and it will be Ark ID look up for up coming traffic and the landing page. With this, the back-end operations interface will be placed behind the VPN for security measures. 

## Installation

Filled out the Mysql database credentails at `config/MysqlArkConf.php` to have the resolver connected to exsiting Ark IDs database. 

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


