# sass-repository

Sass-repository is a sass module you can use in your project as a node module. It consists of:
  - One grid system;
  - Some common usefull helpers;
  - A flexible css and sass variables ... *You can use the framework variables
    plus your own variables and they are all accessible via javascript.*
    
    for example: use `f.$my-var` as a scss variable or `f.p(my-var)` as it’s converted to `var(--my-var)`.

  - ...

**Usage:** See `framework/example/package.json`
  - Update/create a package.json in your project to:
    - `$ npm install` to install npm dependencies and sass-repository itself *(dependencies: autoprefixer, npm-run-all, postcss-cli, sass)*
    - Configure the package.json scripts pathes to match your project requirements *(css and sass directories)*;

  - Copy `node_modules/sass-repository/framework/_sample-styles.scss` file to your project sass directory;
  - Run `$ npm run sass:watch` and start editing your project styles.

  - In `project-roote-styles.scss` Configure the framework sass variables.
    include and use the framework mixins you need.
    In this file you can also import your project sass files. Like: *vendors/, layouts/ or themes/* ...

    ```
    /
    | - sass/
      | - project-roote-styles.scss
      | - vendors/
      | - layouts/
      | - themes/
      | - (...)
    ```

    Read more: [Structuring sass projects](https://itnext.io/structuring-your-sass-projects-c8d41fa55ed4)

**More about sass modules**
  - [sass-lang.com](https://sass-lang.com/documentation/at-rules/use)
  - [css-tricks.com](https://css-tricks.com/introducing-sass-modules/)

**Todo:**
  - make it usable with [degit](https://github.com/Rich-Harris/degit)
  
