# DandyWavesAngularPrjct

You may find some Error if You not Using the right base

#<base href="http://localhost/<project name>/">
and also .htaccess file should be configured if you use Appache Server

RewriteEngine On
    // If an existing asset or directory is requested go to it as it is
    RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -f [OR]    
    RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -d    
    RewriteRule ^ - [L]    
    # If the requested resource doesn't exist, use index.html    
RewriteRule ^ /index.html

