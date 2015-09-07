# Build files for PHP projects

## Requirements

  * `php`
  * `composer` ([https://getcomposer.org/](https://getcomposer.org/))
  * `phing`

You can install `phing` globally using `composer`.

To install phing, 

## Installation

Copy [build.xml](PHP/build.xml) and [phpunit.xml.dist](PHP/phpunit.xml.dist) file at the root of your php project.

If it's the first time you use it, run `phing install-requirements`.
You should also add composer bin path to your `$PATH`. 
Using linux, you can just run `echo 'export PATH=~/.composer/vendor/bin:$PATH' >> ~/.bashrc` (or `~/.zshrc`).

## Usage

```bash
phing <command>
```

| Command              | Description                                            |
| :------------------- | :----------------------------------------------------- |
| help                 | Shows this help                                        |
| tests                | Run tests for development                              |
| ci                   | Run tests for continous integration                    |
| lint                 | Linter                                                 |
| phpunit              | Executes phpunit tests                                 |
| coverage             | Show phpunit coverage                                  |
| phpcs                | Detects standard violations on the code                |
| phpmd                | Look for several potential problems                    |
| phpcpd               | Detects duplicate code portions                        |
| phpmetrics           | PhpMetrics provides various metrics about PHP projects |
| phploc               | Measure the size and analyze the structure             |
| install-requirements | Install requirements for build                         |

