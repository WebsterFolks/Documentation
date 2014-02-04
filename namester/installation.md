### Namester Whois Installation

---

#### Requirements
Before getting started with installation check if you host meets the requirements:

- PHP >= 5.3.7
- MCrypt PHP Extension
- Port 43 enabled and accessible via PHP function fsockopen

Note: Normally, all these requirements are available in all shared hosts.

#### Installation Instructions
To install this script first you need to generate a key from our key generator tool [Goto Key Generator](http://v5.websterfolks.com/key/generator)

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

