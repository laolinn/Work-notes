# htacess

## not www -> www

&lt;ifmodule mod_rewrite.c&gt;

RewriteEngine On

RewriteCond %{HTTP_HOST} ^dgcargochina.com [NC]

RewriteRule ^(.*)$ http://www.dgcargochina.com/$1 [L,R=301]

&lt;/ifmodule&gt;