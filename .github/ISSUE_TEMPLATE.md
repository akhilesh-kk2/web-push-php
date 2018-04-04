**NOTE**: Please test in a least two browsers (i.e. Chrome and Firefox). This
helps with diagnosing problems quicker.

> Please confirm the following:

- [y] I have read the [README](https://github.com/web-push-libs/web-push-php) entirely
- [y] I have verified in the [issues](https://github.com/web-push-libs/web-push-php/issues) that my problem hasn't already been resolved

# Setup

> Please provide the following details, the more info you can provide the
> better.

* *Operating System*: <Linux>
* *PHP Version*: <5.6>
* *web-push-php Version*: <1.4.0>

> Please check that you have installed and enabled these PHP extensions :

- [y] gmp
- [y] mbstring
- [y] curl
- [y] openssl

> Please select any browsers that you are experiencing problems with:

- [ ] Chrome
- [ ] Firefox
- [ ] Firefox for Mobile
- [ ] Opera for Android
- [ ] Samsung Internet Browser
- [ ] Other

> Please specify the versions (i.e. Chrome Beta, Firefox Beta etc).

# Problem

> Fatal error: Uncaught exception 'RuntimeException' with message 'Curve curve(-3, 41058363725152142129326129780047268409114441015993725554835256314039467401291, 115792089210356248762697446949407573530086143415290314195533631308867097853951) does not contain point (3241839770838454464458762781498604280851602814305279715423694631606457933959, 5171447275398088959133285509003806382170852108135282320327383382674674072772)' in C:\xxxxxxxxx\vendor\mdanter\ecc\src\Primitives\Point.php on line 100

# Expected

> I am using https://github.com/Minishlink/web-push-php-example to send push using VAPID.
In 50% cases code is working fine but in other 50% cases i am getting error. 

# Features Used

- [Y] VAPID Support
- [N] GCM API Key
- [Y] Sending with Payload

# Example / Reproduce Case

> In 50% cases code is working fine but in other 50% cases i am getting error.

# Other

> I also tried to send push using V4, but code throwing new error messages. Please find error message below.

Warning: hex2bin(): Hexadecimal input string must have an even length in C:\xxxxxx\web-push-php-example\vendor\minishlink\web-push\src\Utils.php on line 60

Warning: hex2bin(): Hexadecimal input string must have an even length in C:\xxxxxxxx\web-push-php-example\vendor\minishlink\web-push\src\Utils.php on line 61

Fatal error: Uncaught TypeError: bin2hex() expects parameter 1 to be string, boolean given in C:\xxxxxx\web-push-php-example\vendor\minishlink\web-push\src\Encryption.php on line 94

TypeError: bin2hex() expects parameter 1 to be string, boolean given in C:\xxxxx\web-push-php-example\vendor\minishlink\web-push\src\Encryption.php on line 94
