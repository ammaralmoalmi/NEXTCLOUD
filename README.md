# NEXTCLOUD
NEXTCLOUD

Command of metabase

docker run -d -p 3000:3000 \
--network=odoo_15_default \
--restart=always \
-v metabasedata:/metabase-data \
-e "MB_DB_FILE=/metabase-data/metabase.db" \
-e "MB_DB_TYPE=postgres" \
-e "MB_DB_DBNAME=odoo" \
-e "MB_DB_PORT=5432" \
-e "MB_DB_USER=odoo" \
-e "MB_DB_PASS=odoo" \
-e "MB_DB_HOST=odoo_15_db_1" \
--name metabase metabase/metabase
