Source for [brucebot.com](http://brucebot.com) , a Personal blog about Robotics Automation.

Read the Post [Blog with Jekyll and Markdown](http://brucebot.com/2012/03/blog_with_jekyll_and_markdown/) for more information.(Chinese Only)

##Usage


###instagram/likedphoto

Set your own instagram **access_token** in */instagram/instagram.php* and */likedphoto/
instagram.php*.

`$access_token='Your token';`

###New post

`rake post["post tile",category]`

Automatically Open the new post in default text editor, Mine is [Mou](http://mouapp.com).

There is a `draft` switch for each post, after finish the post, set it to `false` to let jekyll process.

###New Page

`rake write["title"]` 

Automatically Open the new post in default text editor, Mine is [Mou](http://mouapp.com).

###Rake deploy

If you want to do *rake deploy* as I do, add your own remote site info to **Rakefile**

`system "jekyll --rdiscount && rsync -avz --progress --delete _site/ XXX@XXX.com:/home/jekyll/ "`

--EOF--