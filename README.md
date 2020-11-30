<img width="200px" alt="Sass" src="https://rawgit.com/sass/sass-site/master/source/assets/img/logos/logo.svg" />



## This repo contains fully respoosnive static web site editing with Sass. 



**Sass makes CSS fun again**. Sass is the most mature, stable, and powerful professional grade CSS extension language in the world.

Sass is completely compatible with all versions of CSS.Over and over again, the industry is choosing Sass as the premier CSS extension language.

## Install Sass
You can install Sass on Windows, Mac, or Linux by downloading the package for your operating system from GitHub and adding it to your PATH. That’s all—there are no external dependencies and nothing else you need to install. <br>
<a href="https://sass-lang.com/install">More info</a>

## Preporocessing
Once Sass is installed, you can compile your Sass to CSS using the sass command. You'll need to tell Sass which file to build from, and where to output CSS to. For example, running sass input.scss output.css from your terminal would take a single Sass file, input.scss, and compile that file to output.css.

```scss
sass --watch input.scss output.css
```

## Variables
```scss
SCSS SYNTAX
$font-stack:    Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}
```

## Nesting
```scss
SCSS SYNTAX
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```

## Mixins
```scss
SCSS SYNTAX
@mixin btn {
    padding: 10px 40px;
    border: 2px solid $green;
    color: $green;
    background: transparent;
    margin-top: 30px;
    border-radius: 10px;
    font-size: 1rem;
}
 
 button {
     @include btn;
 }
      
```

## Operators
```scss
SCSS SYNTAX
.container {
  width: 100%;
}

article[role="main"] {
  float: left;
  width: 600px / 960px * 100%;
}      
```

## Extend
```scss
SCSS SYNTAX
%equal-heights {
  display: flex;
  flex-wrap: wrap;
}

.message {
  @extend equal-heights;
}
    
```
