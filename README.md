STYLEGUIDE TEMPLATE
-------------------------------------------------------------------------------

##Webpack 4, Sass, HTML5, ES6

Application Installation:
-------------------------------------------------------------------------------
1. Make sure you have node & npm installed (+yarn)
2. Run "npm install"
3. Run "npm run build"
4. Do "npm start"
5. Review what was build in dist/ etc.


Packages
-------------------------------------------------------------------------------
Packages is the folder containing custom themes generated within dist/ directory.
To create a package for marines, or navy, or usace, there is only one import
statement that needs to be updated. Let's work on the example of "usace":

1. Open "src/scss/index.scss" & update the import statement to import "usace"
variables for creating a build:

@import "mixins";
@import "usace/index";
@import "menu";

2. Work with scss files under "src/scss/usace/":

- update your brand and theme colors: theme.scss
- create your variables: variables.scss
- update your css: app.scss

3. Run the build from command-line: "npm run build". A package gets generated
under "dist/". Only take folders, do not transfer "index.html". Copy folders,
now, open "packages/usace", past the folders into the usace package. The HTML file
here is unique to the theme and contains the HTML which is different from
"src/index.html". "packages/usace/index.html" is a modified and customized HTML
version. Always keep it. If you override it, you won't have your theme's content.
If you still override it, make sure you revert in git to the original version.
This html file can be modified, but with thought in mind.

Technologies:
-------------------------------------------------------------------------------
Sass, CSS, HTML5, Ecma2015 (ES6), jQuery Modular JavaScript Programming

Development
-------------------------------------------------------------------------------
Working example with all loaded prototypes into one large flow, website package

Description:
-------------------------------------------------------------------------------
Fully customizable styleguide, variablse for sass can be configured to suit
your template needs.
