# easy-to-use-linux
This is for useful code for easy to useing linux

##This code for using git
To install git

	sudo apt-get install git

To add a Repository and Commit (First create a repository and clone your repository in your pc)

	git status
	git add .
	git commit -m "Your Message"
	git push origin master

##This code for Files permision setup

	ls -al
	pwd
	sudo chmod 775 /home/imtiaz/Sites/public_html/wp-content/themes/sp_coming_soon -R

##Install WordPress in local host
###To install wp-cli use this code

	$ curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
	$ php wp-cli.phar --info
	$ chmod +x wp-cli.phar
	$ sudo mv wp-cli.phar /usr/local/bin/wp

###To install wordpress by wp-cli

	wp --info
	wp core download
	wp core config --dbname='user' --dbuser='root' --dbpass='1234' --dbprefix='wp_'
	wp db create
	wp core install --url='http://localhost/(foulder_name)' --title='site title' --admin_user='user name' --admin_password='your password' --admin_email='your email'
	wp theme status


##how to create site in github

1st 

Create a "New repository"

2nd

clone that site in your pc

3rd

create a html file and push it into origin master

4rd

Now create master gh-pages. to create gh-pages master (use below code)

	git branch gh-pages

To see how much master

	git branch

To go gh-pages branch

	git checkout gh-pages

Now push again into gh-pages

	git push origin gh-pages