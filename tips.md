# 1) Hide Extensions 
### Whe you need hide extensions .php and .html used this code in the new file .htaccess inside project (public_html)

### .php

```
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME}.php -f
RewriteRule ^(.*)$ $1.php
#RewriteRule ^([a-z]+)/?$ $1.php [NC]
```

### .html

```
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME}.html -f
RewriteRule ^(.*)$ $1.html
#RewriteRule ^([a-z]+)/?$ $1.html [NC]
```
