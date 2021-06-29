# jenkins-init-backup
This repository stores files from an initialized /var/lib/jenkins/ folder to easily start a fully ready-made Jenkins server.

Some attributions for users:
 * Jenkins server can be opened at http://localhost:8080 after a successful installation.
 * Initial admin user credentials:
   * Username: admin
   * Password: adminuser
   * (Full name is admin, E-mail address is a fake admin@admin.com address)
   * To prevent security issues, changing admin user's password after your first login is strongly recommended.

How to use this repository content:
 1. Install Jenkins to your OS.
 2. Clone this repo and copy its content into the /var/lib/jenkins/ folder at your system.
 3. The owner of /var/lib/jenkins folder itself and all of its contents must be the "jenkins" user. A "chown jenkins: /var/lib/jenkins/*" command can solve this issue.
 4. Restart Jenkins process (usually you can do it easily with systemd: 'systemctl restart jenkins').
 5. Use your browser to display Jenkins server at http://localhost:8080 (caution: you have to open port 8080 manually!).
 6. Use the credentials above to login the server.
 7. Enjoy...

Have fun :)
