# drupal/pinned-dev-dependencies

This project is for use with a Composer-managed Drupal site. This project is
only needed to run the Drupal test suite on the site, and even then, it is
generally preferable to use the project `drupal/dev-dependencies` instead of
this one.

## Updating

This project is pinned to a specific version of `drupal/core`; it is therefore
slightly more difficult to update if used in conjunction with
`drupal/core-recommended`. Both metapackages must be upgraded
together:
```
$ composer update drupal/core-recommended drupal/pinned-dev-dependencies --with-dependencies
```
If your project is not using `drupal/core-recommended`, then
this project can be upgraded directly:
```
$ composer update drupal/pinned-dev-dependencies --with-dependencies
```
However, it is not recommended to use this project unless you are also using
`drupal/core-recommended`.

## References

This project is derived from the original community project
[webflo/drupal-core-require-dev](https://github.com/webflo/drupal-core-require-dev).
It was generated from tools derived from [webflo/package-generator-drupal](https://github.com/webflo/package-generator-drupal)
and [webflo/package-generator](https://github.com/webflo/package-generator).
