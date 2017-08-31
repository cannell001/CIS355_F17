# CIS355_F17

Configuration settings for fastCG! in php.ini

Set fastcgi.impersonate = 1. FastCGI in IIS supports the ability to impersonate the security tokens of the calling client. This allows IIS to define the security context under which the request runs.

Set cgi.fix_pathinfo=1. cgi.fix_pathinfo provides actual PATH_INFO/PATH_TRANSLATED support for CGI. Previous PHP behavior was to set PATH_TRANSLATED to SCRIPT_FILENAME, and to ignore that setting in PATH_INFO. For more information about PATH_INFO, see the CGI specifications. Setting the PATH_INFO value to 1 will cause PHP CGI to match its paths to the specification.

Set cgi.force_redirect = 0.

Set open_basedir to point to a folder or network path where the content of the Web site is located.
