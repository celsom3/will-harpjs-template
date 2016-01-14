## Will Harp Template - [Demo](http://celsomireles.com)

![Screenshot](screenshot.png)

This is a simple and minimalist template for Harp.js designed for developers that want to write blog posts but don't want to care about frontend stuff.

This was original designed by William Justen as a [Jekyll template](https://github.com/willianjusten/will-jekyll-template), but seeing as how Jekyll was being buggy on my machine, I decided to completely ditch jekyll and develop it with [Harp.js](http://harpjs.com/).

The Theme features:

- Smoothscroll
- Offcanvas Menu
- SVG icons
- About Me page
- Feed RSS
- Sitemap.xml
- Color Customization
- Info Customization

## Basic Setup

1. [Install Harp.js](http://harpjs.com/) with `sudo npm install -g harp`
2. Fork the [Will Harp Template](https://github.com/celsom3/will-jekyll-template.git) (optional, if you want to contribute with improvements)
3. Clone the repo you just forked. `git clone https://github.com/celsom3/will-jekyll-template.git`
4. Edit `_harp/harp.json` to personalize your site.
5. Check out the sample posts in `_harp/posts/` to see examples for assigning categories and tags, and other harp data.
6. Read the documentation below for further customization pointers and documentation.
7. **Remember to compile harp with `harp compile _harp ./` while in the root repo directory.** NOTE: this overrides the README.md file. Still trying to work around that.

## Site and User Settings

You have to fill some informations on `_harp/harp.json` to customize your site.

```
{
	"globals": {
		"title": "Celso Mireles",
		"description": "I write words. About ideas and things.",
		"url": "http://celsomireles.com",
		"username": "Celso Mireles",
		"user_description": "Web Developer and Writer",
		"user_title": "Digital Strategist",
		"email": "celso.mireles@gmail.com",
		"twitter_username": "celsom3",
		"github_username": "celsom3",
		"disqus_username": "celsomireles",

		"links": [
			{
				"title": "Home",
				"url": "/"
			},
			{
				"title": "About Me",
				"url": "/about"
			}
		]
	}
}
```

## Color customization

All color variables are in `src/styl/variable`. To change the main color, just set the new value at `main` assignment. Another colors are for texts and the code background color.

## Creating posts

You can use the `initpost.sh` to create your new posts. Just follow the command:

```
./initpost.sh -c Post Title
```

The new file will be created at `_posts` with this format `date-title.md`.

## Post Data

When you create a new post, you need to fill the post information in the `_data.json` file in the posts directory, follow this example:

```
"2016-01-13-first-pull-request-on-github": {
	"title": "My first Pull Request",
	"date": "2016-01-13 21:32:35 -0200",
	"day": "13",
	"month": "January",
	"year": "2016",
	"description": "Making a big deal out of this.",
	"tags": ["git", "web development", "wordpress"],
	"categories": "Development",
	"twitter_text": "First Pull Request on Github",
	"excerpt": "Today was pretty epic for me. Not gonna lie. At the risk of sounding like a total noob, I will announce that today was the first time I contributed to an open source project. Let me start from the beginning"
}
```

Be sure to add it as the first entry in `_data.json` so that your most recent post will show up first.

## Running the blog in local

In order to run locally, just run:

```
	harp server
```


## Questions

Having a problem getting something to work or want to know why I setup something in a certain way? Ping me on Twitter [@celsom3](https://twitter.com/celsom3) or file a [GitHub Issue](https://github.com/celsom3/will-jekyll-template/issues/new).

## License

This theme is free and open source software, distributed under the The MIT License. So feel free to use this Harp.js theme on your site without linking back to me or using a disclaimer.

If you’d like to give me credit somewhere on your blog or tweet a shout out to [@celsom3](https://twitter.com/celsom3), that would be pretty sweet. Also, this work is forked from Willian Justen's jekyll theme, you can give him some love for the great design as well, [@willian_justen](https://twitter.com/willian_justen).
