
# Semstrap

Semstrap (or "semantic bootstrap") is a collection of CSS styles that add a modern look and feel to web projects. 

It aims to have the convenience of frameworks like [Bootstrap](http://getbootstrap.com/) but using only semantic HTML for styling and vanilla Javascript for interactive widgets.

Many developers turn to frontend frameworks just to easily improve the looks of their web projects. Unfortunately this approach results in a loot of framework-specific code like class names and wrapping elements being added to your HTML. Sometimes you even end up adding a bit of code from a another web project that relies on a different front end framework and you get a mess of dependencies and conflicting class names.

Semstrap styles only targets elements. When you want to use it to style a `form` element you just add the element like so:
```
<form>
    <label for="inputEmail">Email address</label>
    <input id="inputEmail" type="email">
</form>
```
... as opposed to:
```
<form class="form form-modifier">
  <div class="form__wrapper form__wrapper-modifier">
    <label class="form__wrapper__label" for="exampleInputEmail1">Email address</label>
    <input class="form__wrapper__input form__wrapper__input-modifier"" type="email" class="form-control"
  </div>
</form>
```

Check it out on https://iamfrank.github.io/semstrap/

## Using it

If you want to use Semstrap in your project, just download `semstrap.css` [from here](/_site/css/semstrap.css) and add it to your HTML files along with a link to the *Open Sans* font from Google Web Fonts:
```
<link rel='stylesheet' type='text/css' href='https://fonts.googleapis.com/css?family=Lato:400,700'>
<link rel='stylesheet' type='text/css' href='.../semstrap.css'>
```
That's it. Take a look at the [docs](https://iamfrank.github.io/semstrap/) to see the cool stuff you can build with pure HTML elements and Semstrap.


## Build and customize

If you want to have your own version of the documentation pages running, you'll need to install [jekyll](https://jekyllrb.com/), git clone the project and run the serve command from your console.
```
$ git clone https://github.com/iamfrank/semantic-strap.git // Clone the SemanticStrap git project
$ jekyll serve
```
Then go look up http://localhost:4000/ in a web browser.
While running the server, Jekyll watches for changes in the files and rebuilds the. Now you can change any styles you want in the [_sass](/_sass) directory and see them applied to the documentation pages.
