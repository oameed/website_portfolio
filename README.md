#  Creating a Static Website using SSGs

The static site generator (SSG) used for this project is [HUGO](https://gohugo.io/) v0.80 extended. To download and install `hugo`, visit: [hugo releases](https://github.com/gohugoio/hugo/releases). 

## References

[1]. 2017. Camden. Rinaldi. _Working with Static Sites: Bringing the Power of Simplicity to Modern Sites_

_Useful Web Tutorials_

[[2].](https://retrolog.io/blog/creating-a-hugo-theme-from-scratch/) 2020. Lopez. _Creating a Hugo Theme From Scratch_

## Workflow

The following procedure describes how to create a website by first creating a theme and furthur customizing it.  
1. generate a new website directory named `website`:
   * `hugo new site website`
2. `cd` to the `website` directory.
3. generate a new theme named `mytheme`:
   * `hugo new theme mytheme`
4. create the following style file:
   * `website/themes/mytheme/static/css/style.css`
5. get the `bootstrap.min.css` file: 
   * go to [Bootstrap](https://getbootstrap.com/) website.
   * download the _Compiled CSS and JS_ and extract the zip.
   * copy `bootstrap.min.css` to `website/themes/mytheme/static/css` directory.
6. insert the following in `website/config.toml`:
   * `theme="mytheme"`
7. customize `website/config.toml` and the contents of `website/mytheme` directory to arrive at a rough sketch for the intended design. At any point during the entire process, the site can be viewed by:
   * `cd` to `website`
   * `hugo server`
   * on a browser, go to `localhost:1313`
8. with `mytheme` available as a _template_, design can be fine tuned by placing a copy of the theme files to be further edited in the same relative path in project’s root (See Hugo's documentation on [Customize a Theme](https://gohugobrasil.netlify.app/themes/customizing/) for more information). 
9. with the intended design achieved, the following step will generate the website to the `website/public/` directory (See Hugo's documentation on [Basic Usage](https://gohugo.io/getting-started/usage/) for more information):
   * `cd` to `website`
   * `hugo`







