### Namester Whois

<script src="http://v5.websterfolks.com/assets/docs/vendor/holder.js"></script>

---


<img alt="Namester%20Whois" data-src="holder.js/100%x225/namester/text:Namester%20Whois">

Namester Whois lets you find whois data for a wide variety of domains with SEO stats, Meta Info, IP location, DNS Records, Website ScreenShot & many other Stats. It is the most fully fledged whois script built on rock solid Laravel Framework. Simple and easy to use, have it up and running in minutes with no PHP experience. 

<div class="btn-group btn-group-justified">
	<a href="http://v5.websterfolks.com/demo/namester" class="btn btn-info">Demo</a>
	<a href="http://v5.websterfolks.com/support/namester" class="btn btn-success">Get Support</a>
	<a href="http://v5.websterfolks.com/feedback" class="btn btn-info">Give Feedback</a>
</div>


<script>
Holder.add_theme("namester", {background:"#F35A0D", foreground:"#ffffff", size: 0.2}).run()
</script>

<br>

#### Features
- Whois Info, Registrar Details, Registration, Expiry & Last Update Dates. 
- NameServers with IP Details.
- Google Map Location of hosting server with IP and Country. 
- Domain Review with SEO Stats and rankings.
- SEO Stats like Alexa Rank & Google PageRank
- Powerful Admin Control Panel.
- Fully SEO Optimised.
- Website ScreenShots with local storage for superior performance.
- Meta Information like meta title, description & keywords.
- A Clean and Responsive Design that works on all devices.
- Custom Pages with contact form support + STMP support.
- Extremely clean urls for even better SEO.
- Multiple Ad Locations with prefect spots to increase click throughs.
- Spam Protection against various bots.


<br>

#### Requirements 
Before getting started with installation check if you host meets the requirements:

- PHP >= 5.3.7
- MCrypt PHP Extension
- Port 43 enabled and accessible via PHP function fsockopen 

Note: Normally, all these requirements are available in all shared hosts.

<br>

#### Installation Instructions
To install this script first you need to generate a key from our key generator tool [Goto Key Generator](http://v5.websterfolks.com/key/generator/)

Once you have got the key, note it down somewhere safe and follow these steps.

- Unzip files on your computer
- Now edit `app/config/production/app.php` and replace `YOUR_API_KEY_HERE` with the key that you generated before.
- Create a MySQL database at your host.
- Edit `app/config/production/database.php` and fill in your database details like this:

<pre>
	'mysql' => array(
        'driver'    => 'mysql',
        'host'      => 'localhost',
        'database'  => 'YOUR_DATABASE_NAME_HERE',
        'username'  => 'YOUR_USERNAME_HERE',
        'password'  => 'YOUR_PASSWORD_HERE',
        'charset'   => 'utf8',
        'collation' => 'utf8_unicode_ci',
        'prefix'    => '',
	),
</pre>

- You need to change values of only three things here `database`, `username` & `password`.
- Now chmod `app/storage` and all folders under it to 777.
- Open `http://www.yourdomain.com/install` in your browser, provide the asked information and done.


If everything goes good then you should see a success message else [contact support](http://v5.websterfolks.com/support) for help.

<br><br>

### Configuration

---

All basic configurations are possible from config area of your AdminCP i.e. `http://www.yourdomain.com/admin/config`

#### Routes Modification

In case you want to change any routes related to this script you can do this by following these instructions:

- Copy `namester.php` from `app/config` to `app/config/production` directory. 
- Now just change the values for `routes` array to anything you want like this:
<pre>
'routes' => array(
		'whois' 	=> ‘website’, // default is www
		'pages' 	=> 'p', // default is pages
		'admin' 	=> 'a', // default is admin
),
</pre>

#### Number of sites on homepage

To change the number of sites on homepage just change value of `per_page` attribute on in this file, like this:

<pre>
'home'	=> array(
		// How many sites on homepage?
		'per_page'	=> 5, // default is 10
),
</pre>

<br><br>

### Credits

---

We proudly use these PHP Frameworks, Classes, Packages & Various other components in Namester Whois

- [Laravel](http://laravel.com)
- [PHPWhois](https://github.com/WebsterFolks/PHPWhois)
- [BootStrap](http://getbootstrap.com/)
- [Font Awesome](http://fontawesome.io)
- [BootFlat](http://www.flathemes.com/)
- [Journal theme by BootSwatch](http://bootswatch.com/journal/)
- [GuzzlePHP](http://guzzlephp.org)
- [Intervention Image](http://intervention.olivervogel.net/)
