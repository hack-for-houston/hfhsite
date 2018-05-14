# Hack for Houston

It is built using the open source [AMP Start framework](https://www.ampstart.com/) and can be customized as per your requirements.

## What is AMP

AMP stands for [Accelerated Mobile Pages](https://www.ampproject.org/), a Google-backed project designed as an open standard for any publisher to have pages load quickly on mobile devices.

## Adding a page

Lets say we are creating a page called xxx.
- Create a markdown file in the root directory of the project with the name of the page as the name of the file. We create xxx.md.
- Make sure, in the frontmatter section of this file, you set the permalink to the name of the page.
- In _config.yml, add it under additional pages.
- If you want to have it in the navigation bar, go to _data/navigations.yml, and add an entry with the name of the file.


#### Deploying to Github Pages
**Method 1**

Push the contents of _site/ to the gh-pages branch.

## Usage

### _config.yml
Update _config.yml with your respective settings like updating your site's name, description etc...

### Styling
AMP has a limitation that you can only use inline css.
All the CSS for this theme is in the styles.scss file in the includes directory.

#### Changing the Default Color
In the styles.scss file in the includes directory, you can change the hex value of $theme-color to the color you would like your site to use.

### Author Information
Author information is present in the author.yml file in the _data folder. You can update the fields of that file as per your requirements.

### Sidenav
Sidenav can be updated from the navigation.yml file in the _data folder.

## Writing Posts
You can write posts just as you would in Jekyll, the only difference being that AMP has some strict guidelines on including external content.

You cannot use Markdown format or normal HTML tags. AMP provides its own custom tags for images, videos etc...

### Examples -

**Images**
`<amp-img src="welcome.jpg" alt="Welcome" height="400" width="800"></amp-img>`

**Videos**
`<amp-youtube data-videoid="mGENRKrdoGY" layout="responsive" width="480" height="270"></amp-youtube>`

[See Full AMP Documentation.](https://www.ampproject.org/docs/)

### Using AMP Components
Some AMP components require you to specify external scripts before using them.
You can specify these scripts in the head.html file in the includes directory after the already imported scripts and then use these components in any post.

## Validating your page with AMP
AMP provides built-in validator to validate your pages so that they can rendered quickly.

You can access this validator by opening the Developer Console in your browser and adding #development=1 to any url of your site.

Example -
http://localhost:4000/#development=1

If you have errors on your page, AMP will list those for you in the console. If you do not have any errors, you'll get a message "AMP Validation Successful" on your console.

## Enabling Google Analytics
1. Set up your Analytics Tracking ID in _config.yml.
2. Remove {% comment %} and {% endcomment %} tags in the default.html file in layouts directory.

## Thanks
This website is based on [Hanuman](https://github.com/samanyougarg/hanuman) jekyll theme. Thank You.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
