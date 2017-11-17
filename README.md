# uri

[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]

URI manipulation Library for URIs ([RFC3986][1] URL, URN, Windows path, relative path or file)

## Install

### Via Composer

```bash
composer require peterpostmann/uri
```
If you dont want to use composer use the files as described in the sub-projects and include them into your project.

- [php-parse_uri][2]
- [php-resolve_uri][3]
- [php-fileuri][4]

## Usage

~~~PHP

use peterpostmann\uri;

// parse_uri
array uri\parse_uri ( string uri [, int $component = -2 [, bool $convertUrlToUrn = null ]] )

// resolve_uri
string uri\resolve_uri ( string basePath, string newPath ) 
string uri\build_uri ( array components )
string uri\convert_url2urn ( string uri, bool convertUrlToUrn = null )

// fileuri
string uri\fileuri ( string path [, string basePath] ) 

~~~

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[link-travis]: https://travis-ci.org/peterpostmann/php-uri

[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/peterpostmann/php-uri/master.svg?style=flat-square

[1]: https://tools.ietf.org/html/rfc3986/
[2]: https://github.com/peterpostmann/php-parse_uri
[3]: https://github.com/peterpostmann/resolve_uri
[4]: https://github.com/peterpostmann/php-fileuri