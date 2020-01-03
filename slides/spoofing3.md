```php
<?php

$subject = 'You\'re Fired!';
$headers = [
    'From' => 'The Boss <boss@company.com>',
];
$message = 'It\'s been brought to my attention that you\'ve
    been stealing from the company and smell bad.

    I have been left with no other choice but to let you go.
    Please clean out your desk immediately.

    — The Boss';

mail('someone@company.com', $subject, $message, $headers);
```

Note:

The command to send this is pretty simple; fortunately, modern email clients check for special SPF and DKIM records to verify email is coming from who it says its from.
