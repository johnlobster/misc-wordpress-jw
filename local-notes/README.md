# Running WordPress locally

### Installation on laptop

Start Apache and mySql through XAMPP

Run XAMPP through windows menu. Click on Apache start and then mySql start

Note 2/21/2024 If mySql doesn't start, there may be another instance using the same port. Use the NetStat button on XAMPP to see what is happening. If there is a mysql running on port 3036, then go to task manager and end that process

### Sample site creation

I have been having a lot of difficulty remembering site names, database names etc. So here is an example

[Tutorial](https://elementor.com/academy/install-wordpress-xampp/)


Code is at `/c/xampp/htdocs/wpSetupTest2`. Should have unpacked WordPress to this location

Create database. 
Go to php admin screen (click admin on xampp control panel)
Click on databases. Enter db name (`wpSetupTest2`)

Browse to `http://localhost/wpSetupTest2/wp-admin/setup-config.php` for setup

- database: `wpSetupTest2`
- username: `root`
- password: Leave the field black
- database host: `localhost`
- table prefix: `wp_`

Submit

Then another window pops up, general website info, but also ID and password for main admin account
In this case
- UserName: `adminJohn`
- password: `wpAdminJohn`

This is only running locally, so doesn't really matter what the password is

![Setup database](./wp-setup-1.jpg "Setup menu")
![Setup database](./wp-setup-2.jpg "Setup menu")
