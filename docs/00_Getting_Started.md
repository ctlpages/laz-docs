**LAZ** is an social network that is built with open source packages allowing system adminstrators to create robust communities, as well as control the functionality, content and look of their application.

[TOC]


## Getting Started

**This documentation assumes that you have prior experience with web applications and php frameworks expecially [laravel](http://laravel.com)**

It also assumes you:

- are using a unix machine (ubuntu 14.04)


### Install


```bash
composer create-project --prefer-dist ctl/laz <name-of-project>
```
You can also download it from Github master branch

```bash
git clone https://github.com/Core-Tech-Labs/LAZ <name-of-project>

```

#### Composer Package download

Once the project is on your machine you would need to run

``` bash
composer install

```

#### Getting your application running

To successfully run LAZ we advise you use a Virtual Machine (vagrant) or an Instance (AWS EC2, heroku, Digital Ocean) for optimal usage.

SSH into VM or Instance, navigate to project root (most likely `/var/www`) run

```bash
php artisan migrate

```


## Configuration

To configure you would need to look at your .env file and add the required fields for usage.

ie: If your `mysql` information is wrong the application would not work.

### PHP Requirements

Its recommended to use PHP version `7.0.*`

I would not recommended using `HHVM` seeing it proves unstable with php 7.0 projects and packages.

#### Extensions

List of extension that are currently needed for LAZ:
* PHP: `mbstring`, `mysql`, `gd`, `mcrypt`, `curl`, `xsl`

### Redis

For your users to populate their news feed you would need to install redis-server`

check if its installed

```bash
$ redis-server -v
Redis server v=2.8.4 sha=00000000:0 malloc=jemalloc-3.4.1 bits=64 build=a44a05d76f06a5d9
```

if given

```bash
-bash: redis-server: command not found
```

```bash
sudo apt-get install redis-server
```

ie: To learn more about [redis](http://redis.io) and [installing tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-redis)

## Demos

If you are currently using LAZ Framework and want to be featured please email [info@ctlabs.net](info@ctlabs.net)


## Support

If you need help using LAZ, or have found a bug, please create an issue on the <a href="https://github.com/Core-Tech-Labs/LAZ/issues" target="_blank">GitHub repo</a>.
