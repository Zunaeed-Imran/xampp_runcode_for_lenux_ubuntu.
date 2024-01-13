## Ubustu xampp server run problem fixing.
- Modify ACL permissions for htdocs folder for daemon user, when using PHP and using xampp we are gonna need taht.
- `sudo setfacl -Rdm u:daemon:rwx /opt/lampp/htdocs/`
- than rename with same command "daemon" to "imran"
- `sudo setfacl -Rm u:daemon:rwx /opt/lampp/htdocs/`
- than rename "daemon" with "imran"
- finally this command will show details
- `sudo getfacl /opt/lampp/htdocs/`
- Xampp server start command in Ubuntu every single time after turn on the computer
- `sudo /opt/lampp/lampp start`
##### Some resource for this Problem
- 