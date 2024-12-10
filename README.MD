## Ubuntu xampp server run problem fixing.

- Modify ACL permissions for htdocs folder for daemon user, when using PHP and
  using xampp we are gonna need taht.
- `sudo setfacl -Rdm u:daemon:rwx /opt/lampp/htdocs/`
- than rename with same command "daemon" to "imran"
- `sudo setfacl -Rm u:daemon:rwx /opt/lampp/htdocs/`
- than rename "daemon" with "imran"
- finally this command will show details
- `sudo getfacl /opt/lampp/htdocs/`
- Xampp server start command in Ubuntu every single time after turn on the
  computer
- `sudo /opt/lampp/lampp start`
- Xampp server stop command
- `sudo /opt/lampp/lampp stop`
- when apache running SQl database not work so we have to stop apache2 than it
  will work.
- `sudo service apache2 stop`
- another problem in laravel using xampp (Install mbstring Extension (if not installed))
- `sudo apt-get install php-mbstring`
- `sudo service apache2 restart`   # or restart your PHP service

##### Some resource for this Problem (xampp server)

- All link provided by julius Brother.
- [1st Youtube link](https://youtu.be/yVL9UbHN_Z0?si=E3PWD9Ht1d4_BMgN)
- [2nd Youtube link](https://youtu.be/5LNSJYi6ITs?si=4V33rEc2RM3aGEvE)
- [Stack overflow link](https://stackoverflow.com/questions/60678203/is-it-possible-to-use-live-server-for-php-with-autoreload-on-save)
