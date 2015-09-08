# Referrer Spam Blocker
This public repository exists to maintain an updated list of HTTP referrer spam sites in .htaccess and nginx.conf formats. Pull requests are welcomed and encouraged, as new spam sites pop up every day.

### Why Block These Sites?
Referrer spam sites can wreak havoc on your website's analytics. Because the traffic they point to your site is automated, you are unable to get a true picture of your website's activity (without messing around with filters all the time).

### How Does This Work?
Apache and Nginx servers have configuration files (.htaccess and nginx.conf, respectively) that are referenced when a request is made to your server. The files provided in this repository tell your server to check where the request is coming from. If it's one of the known spam sites in this list, it returns a 403 Forbidden response.

### Are These Safe To Use?
Yes, if you know what you're doing. These configuration files can be very powerful, and can certainly cause issues for your website if used incorrectly. Be especially careful that you don't overwrite existing configuration files on your server when you use these, as there's a good chance you'll break things if you do.

### I Downloaded The Repo, But The .htaccess File Isn't There!
Files that begin with a dot are considered hidden files, and will not show up in your finder/explorer/IDE if it is not configured properly. You'll have to update your configuration settings to show hidden files.

### I Have Spam Sites To Add, But I Don't Really Understand This Stuff
That's totally cool! Just [create a feature request](https://github.com/mvanderlinde/referrer-spam-blocker/issues/new) with a list of the sites you'd like added, and we'll do it for you.

### Are You A Wizard?
...