### Namester Whois Installation

---

#### Requirements 
Before getting started with installation check if you host meets the requirements:

- PHP >= 5.3.7
- MCrypt PHP Extension
- Port 43 enabled and accessible via PHP function fsockopen 

Note: Normally, all these requirements are available in all shared hosts.

#### Installation Instructions
To install this script first you need to generate a key from our key generator tool [Goto Key Generator](http://v5.websterfolks.com/key/generator/beta)

Once you have got the key, note it down somewhere safe and follow these steps.

- Unzip files on your computer
- Now edit `app/config/app.php` and search for `YOUR_API_KEY_HERE`. Now replace it with the key that you generated before.
- Create a MySQL database at your host.
- Edit `app/config/database.php` and fill in your database details like this:

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
- Now chmod `app/storage` folder to 777.
- Open `http://www.yourdomain.com/install` in your browser, add all the asked information.


If everything goes good then your should see a success message else [contact support](http://v5.websterfolks.com/support) for help.

