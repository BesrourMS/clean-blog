# Clean-Blog
A clean, Bootstrap blog theme for Pico CMS Designed by [Start Bootstrap](http://startbootstrap.com/template-overviews/clean-blog/)

## Installation under Pico CMS >= 2.0

-	Download the zip file from this location : https://github.com/BesrourMS/clean-blog and unzip it.
-	Copy the folder 'clean-blog-master/clean-blog/' to '/themes'.
-	Backup your '/content' directory somewhere else.
-	Delete all files and folders present in '/content'.
-	Copy the contents of 'clean-blog-master/content-sample' to '/content'.
-	Edit '/config/config.yml' and put this line by replacing previous one: 'theme: clean-blog'
-	Install the '[Pico Pagination Plugin](https://github.com/rewdy/Pico-Pagination)', which allows to show several pages of articles titles. Go to this page to download and install it : https://github.com/rewdy/Pico-Pagination . It is basically just copying one file, very easy.
-	You can now test your blog in your browser it should be showing up properly.


## Installation under Pico CMS < 2.0
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
Install the '[Pico Pagination Plugin](https://github.com/rewdy/Pico-Pagination)', which allows to show several pages of articles titles. Go to this page to download and install it : https://github.com/rewdy/Pico-Pagination . It is basically just copying one file, very easy.Then so you must add this setting to config.php
```sh
$config['pagination_limit'] = 4;
```


Copy index.md & post.md from content-sample to your content folder and change the meta data

## Customization

-	Change the title of the main page by editing the '/config/config.yml' file, in the 'site_title' field
-	Change the desecription that goes just below that title by editing the '/content/index.md' file, in the 'Tagline' field
-	Change the main web page description meta tag by editing the '/content/index.md’ file, in the 'Description' field
-	Change the top picture by adding the picture, with size of 1900x994 pixels, in the '/themes/clean-blog/img' directory. Then, edit the '/content/index.md' file, and for the 'Img :' field put this complete line instead:
Img: themes/clean-blog/img/your-picture.jpg
You can also simply put an URL of a picture if needed.
-	No modification to the '/content/index.md' file except the YML header will be shown, only the articles list is shown
-	You can edit the 'Copyright' information at the botton of the articles list page by editing the '/themes/clean-blog/index.twig' file, in the 'copyright text-muted’ class at the very bottom of the file.
-	Change the number of articles shown in the list on the first page by putting this snippet at the end of your '/config/config.yml’ file (here set to 4):<br>
```
##
# Pico Pagination Plugin
pagination_limit: 4
```

## Adding a new blog article
-	You can create a new blog article by copying the '/content/blog.md’ file to a new file called 'blog-2021-03-04_Article_title.md’.
-	You need to edit that new file by putting the right date in the 'Date :’ field in the YAML header (between the '---' lines at the top of the file), in USA style of writing (e.g. 07 June 2021). This is very important as it will order the articles by desscending date.
-	You also need to edit the 'Title’ and 'Description’ of this new file, which both will be displayed on the blog articles list. You can also add a picture if needed in the 'Img’ field.
-	Add as many articles as you need by creating one such new file per article.
-	There is no need to restart anything, your blog and article should now be displayed properly, and the list of articles be updated too.





## Demo : [link](http://blackrockdigital.github.io/startbootstrap-clean-blog/)

## Screenshot
![Clean-Blog-Screenshot](https://startbootstrap.com/assets/img/screenshots/themes/clean-blog.png)
