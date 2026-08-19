# grid

## What is grid?
`Grid` is a 12-column, responsive grid used to create layout and structure for web pages, websites and applications. Open-source and released under the [MIT licence](https://github.com/hackdanismo/grid/blob/main/LICENSE).

## How to use
Download the `grid.css` or `grid.min.css` stylesheets and add to your web project in the same location as all other CSS stylesheets. It is recommended to use the `grid.min.css` stylesheet for production as this has a reduced file size and has been optimised for production websites.

+ [grid.css](https://github.com/hackdanismo/grid/blob/main/grid.css)
+ [grid.min.css](https://github.com/hackdanismo/grid/blob/main/grid.min.css)

Once downloaded, add the grid stylesheet to the `<head>` section of your `HTML`.

```html
<!DOCTYPE html>
<html lang="en">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="This is where the description for the webpage is placed.">

    <title>Webpage Title</title>

    <!-- Include the grid CSS stylesheet -->
    <link rel="stylesheet" href="grid.min.css">
</html>
```

The `grid` will now be added to your webpage.

The `index.html` file in this repo is to demonstrate the grid structure.

For testing, it is recommended to add the `data-debug="true"` attribute to the opening `<html>` tag to see the border/outline of each grid row and column. This should be removed for production/live websites and applications.

```html
<html lang="en" data-debug="true"> ... </html>
```

## Development

### Clone the repository
To clone the repository locally, use the following terminal commands:

```shell
# SSH
$ git clone git@github.com:hackdanismo/grid.git
# HTTPS
$ git clone https://github.com/hackdanismo/grid.git

# Change directory once the repo is cloned
$ cd grid
```

### Set the Node version
It is recommended to set `Node` to the recommended version. For this [nvm](https://github.com/nvm-sh/nvm) `(Node Version Manager)` is used.

```shell
# This will set the recommended Node version, if installed, using nvm
$ nvm use
```

### Minify the stylesheet
CSS changes should be made inside of the `grid.css` stylesheet file. Once changes are made, the minified file, `grid.min.css` should be updated. The `clean-css-cli` npm package is used to minify the CSS code.

```shell
$ npm run minify:css
```

## Licence
The project is created by `Dan Jackson` and released under the [MIT licence](https://github.com/hackdanismo/reset/blob/main/LICENSE).
