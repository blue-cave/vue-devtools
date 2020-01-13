# vue-devtools

### Manual Installation

**Make sure you are using Node 6+ and NPM 3+**

1. Clone this repo
2. `npm install` (Or `yarn install` if you are using yarn as the package manager)
3. `npm run build`
4. Open Chrome extension page
5. Check "developer mode"
6. Click "load unpacked extension", and choose `shells/chrome`.

### Hacking

1. Clone this repo
2. `npm install`
3. `npm run dev`
4. A plain shell with a test app will be available at `localhost:8080`.

### Testing as Firefox addon

 1. Install `web-ext`

	~~~~
	$ npm install --global web-ext
	~~~~

	Or, for Yarn:

	~~~~
	$ yarn global add web-ext
	~~~~

	Also, make sure `PATH` is set up. Something like this in `~/.bash_profile`:

	~~~~
	$ PATH=$PATH:$(yarn global bin)
	~~~~

 2. Build and run in Firefox

	~~~~
	$ npm run build
	$ npm run run:firefox
	~~~~

	When using Yarn, just replace `npm` with `yarn`.


### Common problems and how to fix

1. Fixing "Download the Vue Devtools for a better development experience" console message when working locally over `file://` protocol:
  1.1 - Google Chrome: Right click on vue-devtools icon and click "Manage Extensions" then search for vue-devtools on the extensions list. Check the "Allow access to file URLs" box.

2. How to use the devtools in IE/Edge/Safari or any other browser? [Get the standalone Electron app (works with any environment!)](https://github.com/vuejs/vue-devtools/blob/master/shells/electron/README.md)


### License

[MIT](http://opensource.org/licenses/MIT)
