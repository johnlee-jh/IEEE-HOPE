# Liebling-IEEE -- John

## This PR has specific handlebar themes for the HOPE page (hope.hbs). The HOPE website and its contents are under HOPE.html.

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

## Deployment
After pushing your branch, make a Pull Request. This will cause a Github Action to trigger and automatically deploy the theme to [https://ghost.andrewkdinh.com/](https://ghost.andrewkdinh.com/) under the name `dev-liebling`. If it looks like the theme did not update, then please head to the admin console at [https://ghost.andrewkdinh.com/ghost](https://ghost.andrewkdinh.com/ghost) and change the theme to `dev-liebling`.
