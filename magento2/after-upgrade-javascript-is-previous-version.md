# After Magento 2 upgrade the javascript files are still the previous version.

After a Magento 2 upgrade we were seeing javascript errors in the admin panel. After investigating it turned out that varnish was caching the javascript files. It was not caching the .html files. You will see that apache is not receiving the request for the javascript files in the access.log.

Solution was to restart varnish and clear browser cache.  ``` systemctl restart varnish ```
