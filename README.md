# travis-config-shared-modules
A module for installing a unified Travis CI .travis.yml configuration file
for testing node.js shared modules. It allows for different configurations by
setting the desired fields under the "install-files.travis" key in the module's
`package.json`.

## Configuration
The following configuration options are currently supported:

### `needPrivateModules`
`needPrivateModules` will pull `NPM_TOKEN` from the pipeline's environment
variables and will set it up for authorized `npm install` calls for private
modules.


## Installation

To configure for the first time, or to update the configuration file, once
all configuration options have been specified in destination module's
`package.json` file, simply:

```sh
npm i -D travis-config-shared-modules
```

