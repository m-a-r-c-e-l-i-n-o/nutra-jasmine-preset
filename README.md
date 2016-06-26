# nutra-jasmine-preset
The "nutra-jasmine-preset" module makes available the [jasmine](http://jasmine.github.io/) behavior-driven testing framework and the [commonjs](https://nodejs.org/docs/latest/api/modules.html) module loader to the [N.U.T.R.A.](https://github.com/m-a-r-c-e-l-i-n-o/nutra) unit test runner.

## Install Preset:
```bash
npm install nutra nutra-jasmine-preset
```

## Add Preset Configuration:
Create a "nutra.config.js" config file in the root of your project and populate it with the following:
```js
// nutra.config.js
module.exports = function( config ) {
  config.set({
    frameworks: ['nutra-jasmine'],
    files: ['specs/**/*.js', 'src/**/*.js'] // Modify to include your own app & spec files
  })
  // For more configuration options, please take a look at:
  // https://github.com/m-a-r-c-e-l-i-n-o/nutra#configuration-anatomy
}
```
