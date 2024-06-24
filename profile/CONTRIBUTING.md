# Olifanton Contributing Guide

Thank you for your interest in developing new functionality in the Olifanton project!

Before you make your first pull-request, we recommend that you familiarize yourself with
the following requirements, which we ourselves adhere to when developing Olifanton components.

## How to

### Setup environment

Prepare your environment for development.

Note that the instructions describe working on *nix systems (Linux and possibly macOS),
development on Windows may be difficult and will not be covered in these instructions.

You'll need:

1. Minimum PHP version: 8.1;
2. `sodium` extension;
3. `hash` extension.

### Fork repository

Make a repository fork in your GitHub account.

### Clone your repository

```bash
git clone git@github.com:<YOUR_GITHUB_NAME>/<reponame>.git
cd <reponame>
```

### Create a `feature/` (or `hotfix/`) branch

```bash
git branch feature/<FEATURE_NAME>
git checkout feature/<FEATURE_NAME>
```

### Create pull request

After implementing your new feature (or hotfix) in your local branch, you should
commit and push changes to your fork repository. After that you can create a pull-request.


## Code style

We follow the code writing style described in the [PSR-12](https://www.php-fig.org/psr/psr-12/) standard.

## PHP version

We are excited to use the new features of the PHP language. But we also want to make it possible
to use Olifanton components for those projects that are not able to upgrade to the latest PHP versions.
Therefore, we are currently using language features from PHP version __8.1__.

## Strict types

For us, PHP's strict type mode is a benefit. Use hinting types wherever possible.
Also, enable strict mode at the start of every script:

```php
declare(strict_types=1);
```

## Exceptions

When writing code, we use Exceptions, not passing an error as a value.

This is incorrect code:

```php
class Foo {
    public function calcSome(): int|bool
    {
        // Calculation fails...
    
        // error...
        return false;
    }
}
```

And this code is correct:
```php
class FooCalculationException extends \Exception {}

class Foo {
    /**
     * @throws FooCalculationException
     */
    public function calcSome(): int
    {
        // Calculation fails...
        throw new FooCalculationException("Error description");
    
        return $calulation;
    }
}
```

## And lastly...

...don't forget that we do it all Just For Fun! YOLO!
