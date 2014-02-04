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
