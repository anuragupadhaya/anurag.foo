+++
author = "Anurag Upadhaya"
title = "How to redirect www to domain apex on Cloudflare pages"
date = "2024-07-29"
description = "How to redirect www to domain apex on Cloudflare pages"
tags = [
    "dns",
    "redirect",
    "cloudflare",
]
+++

Ever since I decided to host my hugo website with CloudFlare pages, where I have the current domain parked as well, I was struggling to correctly configure the DNS records and map `www` subdomain so that it redirects to the domain apex.

I tried fiddling around with Redirect rules, Page rules, A and CNAME records but none of them worked.

**What eventually ended up working for me was to set up a bulk redirect as per the [cloudflare documentation](https://developers.cloudflare.com/pages/how-to/www-redirect/)**

<br>

I had an another wrong configuration wherein I had added my domain including `www` to the hugo site deployed through cloudflare pages (https://www.anurag.foo). To resolve, I first had to remove the domain from pages and then reattach without `www` (https://anurag.foo).

<small>Sources:</small>

https://developers.cloudflare.com/pages/how-to/www-redirect/