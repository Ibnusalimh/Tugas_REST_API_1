Untuk program .htaccess adalah:

RewriteEngine On <br />
RewriteCond %{REQUEST_FILENAME} !-f <br />
RewriteCond %{REQUEST_FILENAME} !-d <br />
RewriteRule ^data/([0-9]+)$ /restapitugas/data.php?id=$1 [L] <br />
RewriteRule ^([^\.]+)$ $1.php [NC,L]
