# WCAG 3 docs wire frames

There are two different techniques for writing and updating the informative documents for WCAG3: 
- editing the markdown files in a markdown editor or online on Github with Preview 
- installing a local development server that can display the markdown output

## Edit the Markdown Files
1. Start in the Code tab of the default Github menu. In the left column under Files, change the default of main to the branch that you want to edit.  Unless you are correcting a small typo, don't edit the main branch.  You probably don't have permissions to do it.
2. In the list of folders under the Files column, select how-to, then outcomes.  


### Creating a new outcome

1. Copy `_template/` in `outcomes/`. Use lower case letters and dashes (-) only for the directory name. This will be the **slug** which will be needed later.

2. In your new directory, rename `_template.11tydata.js` to `new-dir-name.11ty.data.js` where `new-dir-name` is whatever you called the directory.

3. in `outcomes.json` set the `title` to be the short name of the outcome. Examples: `Non-text content`, `Error notification`, etc. Add a 3 - 4 sentence description to `description`. The `index` is a number to help sort outcomes in order. Leave at `0` if you do not know what this should be.

4. Fill out the `.md` files in your new directory

### Create a new method

1. Copy the method template from `outcome/_template/methods/_template` to the `methods` directory of the outcome you are creating a method for

2. Give the copied directory an appropriate name

3. Rename `_template.json` to match the directory name, and update its content. Give the method a `title` (1 - 4 words) and a description (2 - 4 sentences). The `slug` must be the directory name. Use `index` to sort methods.

## Installation of a local development envirnment in Github

**Prerequisites**: This project requires [NodeJS](https://nodejs.org/)

From the repository root, run the following command to install all necessary dependencies:

```sh
npm ci
```

## Local development

To run this project locally, use the following command in the repository's root directory. This will start a server on `http://localhost:8080/`. The server has hot-reload enabled so changes to files will be reflected in the browser immediately. 

```sh
npm run serve
```



4. Fill out the `.md` files in your new directory
