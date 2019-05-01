# 7-1-structure-less

Less structure

```bash
--abstracts
-----variables.less
--base
-----resets.less
-----typography.less
--components
-----_buttons.less
--layout
-----footer.less
-----menu.less
-----section.less
--pages
-----home.less
--partials
-----example-cta.less
--defer.less
--responsive.less
--styles.less
```

I use [Blindfold](https://github.com/jhd3197/Blindfold) to convert the less files to css 

[Blindfold](https://github.com/jhd3197/Blindfold) is an electron app and it create two css file one .css and the other one .min.css and it also use [Autoprefixer](https://www.npmjs.com/package/autoprefixer) so you can forgot about vendor prefixes so here is an example

Before [Blindfold](https://github.com/jhd3197/Blindfold)
```bash
.example {
    display: grid;
    transition: all .5s;
    user-select: none;
    background: linear-gradient(to bottom, white, black);
}
```

After [Blindfold](https://github.com/jhd3197/Blindfold)
```bash
.example {
    display: -ms-grid;
    display: grid;
    -webkit-transition: all .5s;
    -o-transition: all .5s;
    transition: all .5s;
    -webkit-user-select: none;
       -moz-user-select: none;
        -ms-user-select: none;
            user-select: none;
    background: -webkit-gradient(linear, left top, left bottom, from(white), to(black));
    background: -webkit-linear-gradient(top, white, black);
    background: -o-linear-gradient(top, white, black);
    background: linear-gradient(to bottom, white, black);
}
```




