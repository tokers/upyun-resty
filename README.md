# upyun-resty

UPYUN's open source software for OpenResty development.

![](http://iresty.b0.upaiyun.com/assets/upyun-resty.png_/fw/400)

# Table of Contents

* [What is UPYUN](#what-is-upyun)
* [What is OpenResty](#what-is-openresty)
* [Tech Talks](#tech-talks)
  * [201411 Beijing OSC](#201411-beijing-osc)
  * [201511 Beijing OpenResty Con](#201511-beijing-openresty-con)
  * [201608 Guangzhou UPYUN OpenTalk](#201608-guangzhou-upyun-opentalk)
  * [201612 Shenzhen OpenResty Con](#201612-shenzhen-openresty-con)
* [Projects](#projects)
  * [Middleware](#middleware)
    * [Project Slardar](#project-slardar)
  * [Nginx Modules](#nginx-modules)
    * [base64-nginx-module](#base64-nginx-module)
  * [Libraries](#libraries)
    * [checkups](#checkups)
    * [httpipe](#httpipe)
    * [redis-ratelimit](#redis-ratelimit)
    * [17monip](#17monip)
    * [sync](#sync)
    * [ctxdump](#ctxdump)
* [Work at UPYUN](#work-at-upyun)

# What is UPYUN

- website: https://www.upyun.com
- github: https://github.com/upyun
- blog: http://io.upyun.com

# What is OpenResty

- website: https://openresty.org
- github: https://github.com/openresty

OpenResty is a full-fledged web platform by integrating the standard Nginx core, LuaJIT, many carefully written Lua libraries, lots of high quality 3rd-party Nginx modules, and most of their external dependencies. It is designed to help developers easily build scalable web applications, web services, and dynamic web gateways.

# Tech Talks

## 201411 Beijing OSC

- Using ngx_lua in UPYUN ([Slide](http://iresty.b0.upaiyun.com/slides/using-ngxlua-in-upyun.pdf) | [Github](https://github.com/timebug/using-ngxlua-in-upyun)) - @timebug

![](http://iresty.b0.upaiyun.com/assets/using-ngxlua-in-upyun.png_/fw/400)

## 201511 Beijing OpenResty Con

- Using ngx_lua in UPYUN 2 ([Slide](http://iresty.b0.upaiyun.com/slides/using-ngxlua-in-upyun-2.pdf) | [Github](https://github.com/timebug/using-ngxlua-in-upyun)) - @timebug

![](http://iresty.b0.upaiyun.com/assets/using-ngxlua-in-upyun-2.png_/fw/400)

## 201608 Guangzhou UPYUN OpenTalk

- 基于 ngx_lua 的动态服务路由方案 ([Slide](http://iresty.b0.upaiyun.com/slides/%E5%9F%BA%E4%BA%8Engx_lua%E7%9A%84%E5%8A%A8%E6%80%81%E6%9C%8D%E5%8A%A1%E8%B7%AF%E7%94%B1%E6%96%B9%E6%A1%88.pdf)) - @yejingx

![](http://iresty.b0.upaiyun.com/assets/%E5%9F%BA%E4%BA%8Engx_lua%E7%9A%84%E5%8A%A8%E6%80%81%E6%9C%8D%E5%8A%A1%E8%B7%AF%E7%94%B1%E6%96%B9%E6%A1%88.png_/fw/400)

## 201612 Shenzhen OpenResty Con

- OpenResty 在云处理服务器集群中的应用 ([Slide](http://iresty.b0.upaiyun.com/slides/OpenResty%E5%9C%A8%E4%BA%91%E5%A4%84%E7%90%86%E6%9C%8D%E5%8A%A1%E9%9B%86%E7%BE%A4%E4%B8%AD%E7%9A%84%E5%BA%94%E7%94%A8.pdf)) - @yejingx

![](http://iresty.b0.upaiyun.com/assets/OpenResty%E5%9C%A8%E4%BA%91%E5%A4%84%E7%90%86%E6%9C%8D%E5%8A%A1%E9%9B%86%E7%BE%A4%E4%B8%AD%E7%9A%84%E5%BA%94%E7%94%A8.png_/fw/400)

# Projects

## Middleware

### Project Slardar

- github: https://github.com/upyun/slardar

Slardar is a HTTP load balancer based on Nginx and lua-nginx-module, by which you can update your upstream list and run lua scripts without reloading Nginx.

## Nginx Modules

### base64-nginx-module

- github: https://github.com/timebug/base64-nginx-module

This module allows for on-the-fly base64 encode. As same as the standard ngx\_http\_gzip_module.

## Libraries

### checkups

- github: https://github.com/upyun/lua-resty-checkups

Manage Nginx upstreams in pure ngx_lua.

* Periodically heartbeat to upstream servers
* Proactive and passive health check
* Dynamic upstream update
* Balance by weighted round-robin or consistent-hash
* Synchronize with Nginx upstream blocks
* Try clusters by levels or by keys

### httpipe

- github: https://github.com/timebug/lua-resty-httpipe

Lua HTTP client cosocket driver for OpenResty / ngx_lua, interfaces are more flexible.

* HTTP 1.0/1.1 and HTTPS
* Flexible interface design
* Streaming reader and uploads
* Chunked-encoding request / response body
* Sets the timeout for read and send operations
* Limit the maximum response body size
* Keepalive

### redis-ratelimit

- github: https://github.com/timebug/lua-resty-redis-ratelimit

This lua library is a request processing rate limit module for ngx_lua. It is used to limit the request processing rate per a defined key between multiple NGINX instances. The limitation is done using the "leaky bucket" method.

### 17monip

- github: https://github.com/timebug/lua-resty-17monip

ipip.net (predecessor is 17momip) ipdb parsing library for OpenResty / ngx_lua. IP query based on ipip.net.

### sync

- github: https://github.com/upyun/lua-resty-sync

This lua-resty library help you to synchronize data(from redis, mysql, memcached and so on) based on the version changes.

It will check the freshness by comparing the version cached by itself(stored in shared memory) and the one from your external suits, data will be updated when the cached one is stale or for the first time.

### ctxdump

- github: https://github.com/tokers/lua-resty-ctxdump

Stash and apply the old ngx.ctx for avoiding being destoried after Nginx internal redirect happens.

# Work at UPYUN

- See more: http://io.upyun.com/join-our-team/
