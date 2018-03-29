![cf](https://i.imgur.com/7v5ASc8.png) Lab 34: UI Styling
======

## Submission Instructions
* Continue working on the fork that you created yesterday
* Create a new branch for all of today's code
* Write all of your code in a directory named `lab-` + `<your name>` **e.g.** `lab-susan`
* Open a pull request to this repository
* Submit on canvas a question and observation, how long you spent, and a link to your pull request

## Configuration
Configure the root of your repository with the following files and directories. Thoughtfully name and organize any additional configuration or module files.
* **README.md** - contains documentation
* **.gitignore** - contains a [robust](http://gitignore.io) `.gitignore` file
* **.eslintrc.json** - contains the course linter configuration
* **.eslintignore** - contains the course linter ignore configuration
* **.babelrc** - contains babel config
* **package.json** - contains npm package config
* **webpack.config.js** - contains webpack config
* **src/** - contains the frontend code
* **src/components/** - contains your components
* **src/main.js** - contains the entire app
* **src/style** - containing your `.scss` partials and styles
* **src/style/main.scss** - contains the entry point for `.scss` partials

## Feature Tasks
##### Minimum Requirements
Style your entire budget tracker app and test your actions!

### Styling
Your application styles should meet the following requirements:
  * all component styles should be contained within a related `.scss` partial
  * all component styles should be imported into the component's `index.js` file
  * all generic base, element, and layout styles should be organized as follows:

```javascript
style
  - lib
    - _vars.scss
  - base
    - _reset.scss
    - _base.scss
  - layout
    - _header.scss
    - _footer.scss
    - _content.scss
```

Your "_vars" partial should contain *at least* the following variables:
  * `$primary` - primary app color
  * `$secondary` - secondary app color
  * `$btn-primary` - primary button color
  * `$gutter` - generic padding/margin gutter for formatting

## Stretch Goals
Use `@extend` to extend an elements styles and apply to another element and create a custom mixin for the handling of vendor prefixes.  For example (you may not use the mixin below as part of the completion of your strecth goals):

```javascript
@mixin border-radius($radius) {
  -moz-border-radius: $radius;
  -webkit-border-radius: $radius;
  border-radius: $radius;
}
```
