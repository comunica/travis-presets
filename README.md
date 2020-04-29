# Comunica Travis Presets

This is a repository for reusable configs for [Travis CI](https://travis-ci.com/),
which can be [imported into your Travis file](https://docs.travis-ci.com/user/build-config-imports/).

## Available Presets

All these presets extend from [`rubensworks/travis-presets:node-base.yml`](https://github.com/rubensworks/travis-presets/blob/master/node-base.yml).

* `yarn.yml`: Uses Yarn for running `build`, `lint` and `test-ci`.
* `yarn-monorepo.yml`: Uses Yarn for running `build`, `lint`, `test-ci` and `coveralls-ci`, and Lerna for running `browser` and `spec`. Also deploys documentation and available Docker images.

## Example

```yml
import: comunica/travis-presets:yarn.yml@master
# ... other stuff
```

## License
This software is written by [Ruben Taelman](http://rubensworks.net/).

This code is released under the [MIT license](http://opensource.org/licenses/MIT).

