# security.txt

When security risks in web services are discovered by independent security researchers who understand the severity of the risk, 
they often lack the channels to disclose them properly. As a result, security issues may be left unreported. 
security.txt defines a standard to help organizations define the process for security researchers to disclose security vulnerabilities securely.

# Nginx config snippet
With this configsnippet, we create a base configuration being able to send a standardized security.txt accross all endpoints
by means of catchall for /security.txt and /.well-known/security.txt

To facilitate host-based parts, you can create a map inside your http block to populate certain fields which can be used to create output

# Minimum Configuration
Download the config-snippet file and load it for the sites you want to apply this for.
Change the snippet and configure it appropriately by populating fields.
If you leave it as is, it will give an empty string / fields when requesting it.

/etc/nginx/snippets/security.txt.conf is then the file to include :)

#License & Copyright
No clue where I got the initial idea from to simply put it like this, If you know, please let me so I can attribute them :) Otherwise, great minds think alike or something ^^
