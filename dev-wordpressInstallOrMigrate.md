**Install WordPress**
1. Created DB and User
1. `wget https://wordpress.org/latest.tar.gz` // pull latest version of WordPress
1. `tar -xzvf latest.tar.gz` // unzip
1. `cd wordpress`
1. `mv * .[^.]* ../` // move files up a directory
1. `cd ../`
1. `rm -rf wordpress` / remove empty folder
1. `rm -rf latest.tar.gz` / remove zip file

**Migrate WordPress**
1. Create new DB on server
1. `mysqldump -u{user} -p{password} {original_db_name} > {dump_db_name}.sql` // Copy DB from original site
1. `mysql -u{user} -p{password} {new_db_name} < {dump_db_name}.sql` // Push DB to new server
1. Update url of DB if this information has changed
   1. `UPDATE wp_options SET option_value = REPLACE(option_value, 'old-url', 'new-url');`
   1. `UPDATE wp_postmeta SET meta_value = REPLACE(meta_value, 'old-url', 'new-url');`
   1. `UPDATE wp_posts SET guid = REPLACE(guid, 'old-url', 'new-url');`
   1. `UPDATE wp_posts SET post_content = REPLACE(post_content, 'old-url', 'new-url');`
1. Reset permalinks to proper syntax and save // if needed

**Migrate WordPress Duplicator**<br>
*Typically in place of the above method I use the [Duplicator plugin](https://wordpress.org/plugins/duplicator/), personally I find this method easier*
1. Source Site:
   1. Install Duplicator
   1. Create Duplicator package on source site
   1. Download files
1. Destination Site:
   - Create blank database and database user
   - Upload to destination server via FTP
1. Browser:
   - Run installer in browser {https://{siteurl}/installer.php
   - Enter DB, DB user and password
   - When done login with the credentials from the source site
   - Note: If you get an error using the link provided just go to the browser and type in the correct URL to the new site
 