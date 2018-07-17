# Gulp | LESS | SCSS | JS
Automate your LESS/SCSS task and bundle your JS scripts with Gulp.js

**Step 1: Install Node.js**

We need Node.js to run Gulp. Node.js can be download from [http://nodejs.org/eng](http://nodejs.org/eng)
Open the command prompt in your system and enter following command.

    node -v
This will display the installed Node.js version.

    npm -v
The version of npm which is used to install modules.

**Step 2: Setup your Gulp Project with npm packages**

When you’re done with installing Node, Download Project from GitHub or clone project to your machine.

    git clone https://github.com/03bgls25/gulp-less-scss-js.git
Now install npm packages listed on package.json file by using following command in the command prompt. Adding “–g” flag ensure that the Gulp is globally available for any project.

    npm install

**Step 3: Configure your Gulp Project**

Open *gulpfile.js* file. Then you can configure you project directory of source and destination path by changing *var config*.

    var config = {
        paths: {
            src: {
                scss: './src/scss/',
                less: './src/less/',
                scripts: './src/scripts/',
            },
            dest: './docs/',
        },
        serve: {
            proxy: '',
            server: './docs/'
        }
    };

**Step 4: Run Gulp task**

You can run your Gulp project by entering following command

    gulp

    gulp serve
