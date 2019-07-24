# Verystream

It's just a php client of the [verystream.com](https://verystream.com/) service.

## Install

```
composer require ainzz/verystream
```

## Usage

All api features are implemented, from retrieve account info

```php
<?php

include_once './vendor/autoload.php';

use ainzz\verystream\verystreamClient;

$verystream = new verystreamClient('apiLogin', 'apiKey');

$accountInfo = $verystream->getAccountInfo();
echo $accountInfo->getEmail(); //account@email.com
```

to upload a file

```php
<?php

include_once './vendor/autoload.php';

use ainzz\verystream\verystreamClient;

$verystream = new verystreamClient('apiLogin', 'apiKey');

$verystream->uploadFile('/home/user/Pictures/image.jpg');
```

It's also possible find more about what you can to do at [verystream API](https://verystream.com/api).

## Author

Alin Stefan

## License

MIT

## Info
Initially forked from Ideneal/OpenLoad 
