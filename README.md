<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Cors Proxy for YunoHost

[![Integration level](https://dash.yunohost.org/integration/cac-proxy.svg)](https://dash.yunohost.org/appci/app/cac-proxy) ![Working status](https://ci-apps.yunohost.org/ci/badges/cac-proxy.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/cac-proxy.maintain.svg)

[![Install Cors Proxy with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=cac-proxy)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Cors Proxy quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Cookie Aware Cors Proxy is an http proxy letting the browser itself manages cookies and redirects.
Most other cores proxy directly respond to redirects, and doesn't send cookies, thus breaking the flow.

With Cookie Aware Cors Proxy, you can call a website not supporting CORS from your own web application, and get the html result.

### Features
- Translates cookies and redirect locations from the target website to have the browser continue to call the proxy and not directly the website 
- Extensive and dynamic support for log and debug information
- Two engines: a lightweight and one based on chrome to support websites running javascript


**Shipped version:** 1.2.0~ynh1

## Screenshots

![Screenshot of Cors Proxy](./doc/screenshots/fnac-logs.png)

## Disclaimers / important information

* About security
    * Single-sign on or LDAP are not integrated
    * It works only if you define it as public upon installation otherwise the yunohost SSO will interfere


## Documentation and resources

* Upstream app code repository: <https://github.com/gcollin/cookie-aware-cors-proxy>
* YunoHost documentation for this app: <https://yunohost.org/app_cac-proxy>
* Report a bug: <https://github.com/YunoHost-Apps/cac-proxy_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/cac-proxy_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/cac-proxy_ynh/tree/testing --debug
or
sudo yunohost app upgrade cac-proxy -u https://github.com/YunoHost-Apps/cac-proxy_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
