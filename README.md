# frappe-codespaces-backup 

https://manual.buildwithhussain.dev/installation/codespaces/  
Install the apps that you want before executing bench start in step 5  

bench switch-to-branch version-15 frappe  
bench update --requirements  
bench migrate  

bench get-app erpnext --branch version-15  
bench --site dev.localhost install-app erpnext  
bench --site dev.localhost migrate  
  
bench get-app hrms  --branch version-15  
bench --site dev.localhost install-app hrms  
bench --site dev.localhost migrate  
  
bench get-app healthcare  --branch version-15  
bench --site dev.localhost install-app  healthcare  
bench --site dev.localhost migrate  
  
bench --site dev.localhost backup --with-files  

bench --force --site dev.localhost  restore  /workspace/frappe-bench/sites_new/dev.localhost/private/backups/(database.sql.gz)   --with-private-files  /workspace/frappe-bench/sites_new/(dev_localhost-private-files.tar)  --with-public-files  /workspace/frappe-bench/sites_new/dev.localhost/private/backups/(dev_localhost-files.tar)


https://github.com/frappe/frappe/wiki/App-Development-using-GitHub  
