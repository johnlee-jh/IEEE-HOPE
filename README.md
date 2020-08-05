# Liebling-IEEE -- John

## HOPE Specific Files
This PR has specific handlebar themes for the HOPE page (hope.hbs, hope.html, and hope.css)

hope.css is added into assets/css/ and the html body of hope.html is inserted into hope.hbs

Adding a category in routes.yaml to direct /hope/ to the hope.hbs template should make the hope page work

The HOPE website and its contents are under hope.html (for backup).

## How to Install Ghost for Development
1. Download NodeJS
2. Verify that you have NodeJS by running `npm --version`
3. Run `sudo npm install -g ghost-cli@latest`. This installs the latest version of the ghost-cli. **NOTE** You must run this with `sudo`. If you are using Windows, you can install this by running an elevated command prompt and running `npm install -g ghost-cli@latest`.
4. Verify that you have Ghost installed by running `ghost --version`
5. Create an empty directory (this is where the ghost development environment will be) and `cd` into it
6. Run `ghost install local --no-start` and check to see whether or not the folder is populated with files
7. Navigate to `your_ghost_folder->content->themes`
8. While inside of the themes folder, clone this repo.
9. Exit back to `your_ghost_folder` and then run `ghost start --development`
10. Go to the specified admin console link (it should be a localhost). Make an account and login.
11. Go to Design under Settings and scroll down to see where the themes are. Activate the `liebling-ieee` theme.
12. Modifications to the theme will change the page. **Before adding your own changes, make a new branch!**

## How to Modify the Theme
When you modify a file within your current theme, you will have to reload the page to see your changes. For help on actual development, see [https://ghost.org/docs/api/v3/handlebars-themes/](https://ghost.org/docs/api/v3/handlebars-themes/).
