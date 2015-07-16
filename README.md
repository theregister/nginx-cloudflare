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

# How to generate

If you don't trust me - and you shouldn't - you can regenerate the `cloudflare.conf` file by executing:

    ./update

You'll need Perl and Mojolicious installed.

That's all, folks!
