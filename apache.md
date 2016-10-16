# Apache

## Redirect using .htaccess file

Source: http://blog.richbeales.net/2012/09/create-generic-www-redirect-app-for.html

```
RewriteEngine On
RewriteCond %{HTTP_HOST} monkeymatters\.com
RewriteRule ^(.*)$ http://stores.ebay.com/monkeymatters [R=301]
```
