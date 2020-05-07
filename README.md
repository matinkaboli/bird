# bird

Framework for web (it's my personal template for starting a new web project :D )

Clone the project using `git clone https://github.com/amovah/bird.git` command.

Then install the dependencies using `yarn install` command, and:

```[sudo] npm install -g gulp nodemon```

Remember, you must have MongoDB installed on your machine.

And to run the project, run `gulp full:dev && npm run devserver` command.

[Contributing](https://github.com/amovah/bird/blob/master/CONTRIBUTING.md)


If you want to make any changes or build the project, you have three ways:


1. `npm run client:build` that just watches `/src/views` and `/src/public/`
2. `npm run server:build` that watches other directories than `src/views` and `/src/public/`
3. `npm run full:build` that watches all of the directories in `src/` dir.

### Router

To add routers, you should create a file in `src/routers/` directory, the simplest way is to write `./bird router ROUTERNAME` in command line.

### Model(Database Collections)

To add collecions, you should create a file in `src/models` directory, the simplest way is to write `./bird model MODELNAME` in command line.

### Public Files

To add CSS, JavaScript, Fonts or Images you should put them in `src/public` file.

Note: CSS files must have .less extension in `/src/public/css/`, except `/src/public/css/lib/` that must have .css

### Utilities

To add utilities you should add files to `src/utils/`

### View

To add html files you should add them to `/src/views/`

Note: In this project we're using nunjucks template, so your files must have .njk extension

### Permissions

To add a permission, add the file to `src/perms/`

## Before you push

Make sure that your files are lint.

You can lint js files in `src/public/js` files using `gulp client:lint` command.

And Other JS files using `gulp server:lint` command.
