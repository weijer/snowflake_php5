# snowflake

[ENGLISH](../README.md) | [中文](README_ZH_CN.md)

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Total Downloads][ico-downloads]][link-downloads]

![](https://cdn.yiranzai.cn/images_upload/20190323175258.png)

这个包生成 64 位 ID，使用来自 Twitter 的雪花算法。

## 目录

```
src/
tests/
```

## 安装

Via Composer

```bash
$ composer require yiranzai/snowflake
```

## 使用

```php
$id = \Yiranzai\SnowFlake\SnowFlake::next($dataCenterId = 1, $workerId = 2);
$node = \Yiranzai\SnowFlake\SnowFlake::analysis($id);

echo $node->dataCenterID; // 1
echo $node->workerID; // 2
```

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## 测试

```bash
$ composer test
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) for details.

## 安全

If you discover any security related issues, please email wuqingdzx@gmail.com instead of using the issue tracker.

## Credits

-   [yiranzai][link-author]
-   [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/yiranzai/snowflake.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/yiranzai/php-snowflake/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/yiranzai/php-snowflake.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/yiranzai/php-snowflake.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/yiranzai/snowflake.svg?style=flat-square
[link-packagist]: https://packagist.org/packages/yiranzai/snowflake
[link-travis]: https://travis-ci.org/yiranzai/php-snowflake
[link-scrutinizer]: https://scrutinizer-ci.com/g/yiranzai/php-snowflake/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/yiranzai/php-snowflake
[link-downloads]: https://packagist.org/packages/yiranzai/snowflake
[link-author]: https://github.com/yiranzai
[link-contributors]: ../../contributors
