# update
Works with the current latest version 0.7.5

# bulma-megamenu
Bulma extension to make Mega Menu. 

<a href="https://codepen.io/hunzaboy/pen/yoPKQW">Click here for Codepen Demo</a>


[![mega-menu.jpg](https://s11.postimg.org/64s8v1ezn/mega-menu.jpg)](https://postimg.org/image/tvrmd5f6n/)

Usage
---
```html
<nav class="navbar ">
....

 <div class="navbar-item has-dropdown is-hoverable is-mega">
        <div class="navbar-link">
          Blog
        </div>
        <div id="blogDropdown" class="navbar-dropdown">
          <div class="container is-fluid">
            <div class="columns">
              <div class="column">
                <h1 class="title is-6 is-mega-menu-title">Sub Menu Title</h1>
                <a class="navbar-item" href="/2017/08/03/list-of-tags/">
                  <div class="navbar-content">
                    <p>
                      <small class="has-text-info">03 Aug 2017</small>
                    </p>
                    <p>New feature: list of tags</p>
                  </div>
                </a>
                <a class="navbar-item" href="/2017/08/03/list-of-tags/">
                  <div class="navbar-content">
                    <p>
                      <small class="has-text-info">03 Aug 2017</small>
                    </p>
                    <p>New feature: list of tags</p>
                  </div>
                </a>
                <a class="navbar-item" href="/2017/08/03/list-of-tags/">
                  <div class="navbar-content">
                    <p>
                      <small class="has-text-info">03 Aug 2017</small>
                    </p>
                    <p>New feature: list of tags</p>
                  </div>
                </a>
              </div>        
              <div class="column">...</div>
              <div class="column">...</div>
              <div class="column">...</div>
            </div>
          </div>
...
</nav>
```

Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `megamenu.scss`
- Copy the code from the `bulma-megamenu repo`'s [megamenu.scss](https://raw.githubusercontent.com/hunzaboy/bulma-megamenu/master/megamenu.scss) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"

@import "megamenu.scss"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
