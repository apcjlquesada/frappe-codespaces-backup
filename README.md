# frappe-codespaces-backup 

https://manual.buildwithhussain.dev/installation/codespaces/

bench get-app erpnext
bench get-app --branch version-15 erpnext
bench --site dev.localhost install-app erpnext
bench --site dev.localhost migrate

bench get-app hrms
bench --site dev.localhost install-app hrms
bench --site dev.localhost migrate

bench get-app healthcare
bench --site dev.localhost install-app  healthcare
bench --site dev.localhost migrate

bench --site dev.localhost backup --with-files

