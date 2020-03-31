# Clean-Blog
A clean, Bootstrap blog theme for Pico CMS Designed by [Start Bootstrap](http://startbootstrap.com/template-overviews/clean-blog/)

## Installation
Download the clean-blog folder, upload it in the themes folder of your pico installation and change the following setting within your config.php:
```sh
 $config['theme'] = 'clean-blog'; 
 $config['pages_order_by'] = 'date';
 $config['pages_order'] = 'desc';
```

You must add these custom settings in your config file 
```sh
$config['author'] = 'Your Name';
$config['facebook'] = 'https://www.facebook.com/YourPage';
$config['twitter'] = '@username';
```
For the pagination I use [Pico Pagination Plugin](https://github.com/rewdy/Pico-Pagination) so you must add this setting to config.php
```sh
$config['pagination_limit'] = 4;
```
For Pico CMS >= 2.0 add to config/config.yml
```sh
theme: clean-blog
```
(If the file does not exist, create it. For more info see config/config.yml.template)
### Home Page & Post Page
Copy index.md & post.md from content-sample to your content folder and change the meta data

### Demo : [link](http://blackrockdigital.github.io/startbootstrap-clean-blog/)

### Screenshot
![Clean-Blog-Screenshot](https://startbootstrap.com/assets/img/screenshots/themes/clean-blog.png)
