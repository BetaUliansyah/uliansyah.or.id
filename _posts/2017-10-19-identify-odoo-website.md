---
layout: post
title:  "Easy way to identify Odoo website"
date:   2017-10-19 00:00:00 +0700
categories: jekyll update
---
From so many ways to identify whether a website is using Odoo or not, I have a special technique. It is very easy and not require any technical experience. Just open up your browser and add `/jsonrpc` to a URL. For example: [https://www.odoo.com/jsonrpc](https://www.odoo.com/jsonrpc). A default odoo installation will response with recognizable error message: 
>`<function RPC.jsonrpc at 0x7f51dfc01268>, /jsonrpc: Function declared as capable of handling request of type 'json' but called with a request of type 'http'` 

![Identify Odoo with /jsonrpd](https://raw.githubusercontent.com/BetaUliansyah/BetaUliansyah.github.io/master/img/odoo-identify.jpg)

If the website is using Odoo, it will return a **Bad Request** response.  Otherwise, it will return a usual 404 error page.