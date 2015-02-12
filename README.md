# nginx-cloudflare

Smallest nginx configuration to support Cloudflare

IP addresses taken from:

https://www.cloudflare.com/ips

# How to use

Copy this file over to `/etc/nginx`

    sudo cp cloudflare.conf /etc/nginx/cloudflare.conf

Then, simply include this in the block which identifies a server you're serving
behind cloudflare, i.e.

    server {
        # ...
        include cloudflare.conf
        # ...
    }

That's all, folks!
