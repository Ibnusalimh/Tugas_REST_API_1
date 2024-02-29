Untuk program .htaccess adalah:

RewriteEngine On__
RewriteCond %{REQUEST_FILENAME} !-f__
RewriteCond %{REQUEST_FILENAME} !-d__
RewriteRule ^data/([0-9]+)$ /restapitugas/data.php?id=$1 [L]__
RewriteRule ^([^\.]+)$ $1.php [NC,L]__
