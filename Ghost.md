Installation on WebFaction: 

- Navigate to Domains/Websites > Applications > Add new application, then choose Ghost for App Category.
- Navigate to Domains/Websites > Websites, choose an existing site, click Add an application, then select the app you just added.
- SSH into your server and cd to the Ghost directory.
- Edit ghost/config.js and change the value for url.
- Cd into the bin directory, then run `./stop && ./start`.
- Go to your-ghost-blog/ghost to access the admin site and set up your account.

Make blog private:

Enter the admin site, choose Settings > General, and check "Enable password protection"
