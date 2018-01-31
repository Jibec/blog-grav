# blog-grav
Un POC of my own blog, using grav CMS

## Run the website

* Download grav https://getgrav.org
* Copy `user` folder and `make_trans`in your grav folder
* Run `php -S localhost:8080 system/router.php` (note, they are some requirements, see project's documentation)
* Access website: http://localhost:8080/admin (use jibec/jibec)

Please note you also need a recent version of po4a to have good markdown support.
I'm using v0.52. If markdown generation doesn't work well, download it from https://github.com/mquinson/po4a/releases
and edit the make_trans script to add a relative path to the po4a binary.

## What should you see?

My blog is written in French, the website is configured to use both French and English.

The script `make_trans` will generate pot/po files from french content.
You may edit translation, run again `make_trans` and see the updated result.

You should be able:

 * to switch from French to English in every existing or newly created pages.
 * to create language agnostic links between pages (link to folder name)
 * to write an english page with no French translation (name will be item.en.md or default.en.md depending on the template you wish to use)
 * to edit the english translation (edit po file with Localize or Poedit) and see the updated content

## My opinion

It works fine! But it doesnt fit my needs regarding to my blog.

It requires php and I need static website to host it in https://jibecfed.fedorapeople.org/blog/.

As far as I know, there is no RSS feed using tag or category, which is mandatory for some blog aggregator (planets).
