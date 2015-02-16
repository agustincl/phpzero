## Crear directiva VirtualHost en Apache (2/2)

    <VirtualHost *:80>
        ServerAdmin admin@admin.com
        DocumentRoot "absolute/path/to/the/project/document-root" # In your machine
        ServerName your.new.server.name.domain.name
        ErrorLog "logs/your.new.server.name.domain.name-error.log"
        CustomLog "logs/your.new.server.name.domain.name-access.log" common
        <Directory "absolute/path/to/the/project/document-root">
            Options Indexes FollowSymLinks
            AllowOverride All
            Order allow,deny
            Allow from all
        </Directory>
    </VirtualHost>