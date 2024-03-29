# Helper to get MIME type in PHP

The current PHP `mime_content_type` returns the MIME content type for a file as determined by using information from the magic.mime file. It might be `text/plain` for file type like css or javascript


This implementation using a map/dictionary of file extension to parse file type content (Original from  [svogal](https://www.php.net/manual/en/function.mime-content-type.php#87856))


## Usage

```php

require_once __DIR__ . '/vendor/autoload.php';

$file_path = './path/to/file.js';
$mime_type = VNAppMob\ExtMimeType::getMimeContentType($file_path);
...

```