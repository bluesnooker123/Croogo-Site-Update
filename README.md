# Croogo-Site-Update
Update site using Croogo

Croogo is a CakePHP powered Content Management System.

To Edit website which was built using Croogo you have to login to the grasp pake like below:

https://warwickestates.net/grasp/

To display a RSS Feed with PHP please refer this: [https://bavotasan.com/2010/display-rss-feed-with-php/]

To fix bug for iframe 403 error in PHP, CakePHP (including Croogo), Please refer this: [https://forum.ait-pro.com/forums/topic/bbpress-bulk-user-edit-403-error-user-edit-php-403-error/]

For example:

If you see Error Message: "Forbidden 403 Access to this resource on the server is denied" then it is because you were spot on about mod_security. 

Even though I had disabled it through the VPS, the site was somehow still running it until I added this to the .htaccess file:

<IfModule mod_security.c>
SecFilterEngine Off
SecFilterScanPOST Off
</IfModule>
