# drupal/core-recommended-dev-dependencies

This project is for use with a Composer-managed Drupal site. This project is
only needed to run the Drupal test suite on the site. Most sites probably do
not need to use this project.

## Updating

This project is pinned to a specific version of `drupal/core`; it is therefore
slightly more difficult to update if used in conjunction with
`drupal/core-recommended-dependencies`. Both metapackages must be upgraded
together:
```
$ composer update drupal/core-recommended-dependencies drupal/core-recommended-dev-dependencies --with-dependencies
```
If your project is not using `drupal/core-recommended-dependencies`, then
this project can be upgraded directly:
```
$ composer update drupal/core-recommended-dev-dependencies --with-dependencies
```

## References

This project is derived from the original community project
[webflo/drupal-core-require-dev](https://github.com/webflo/drupal-core-require-dev).
It was generated from tools derived from [webflo/package-generator-drupal](https://github.com/webflo/package-generator-drupal)
and [webflo/package-generator](https://github.com/webflo/package-generator).
