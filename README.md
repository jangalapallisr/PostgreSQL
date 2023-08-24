# PostgreSQL
postgresql




https://www.postgresqltutorial.com/postgresql-cheat-sheet/


postgres=# select setting from pg_settings where name = 'data_directory’;
/var/lib/postgresql/12/main
subbuj@postgres-dpt-test:~$ ls -ltr /etc/postgresql/12/main/postgresql.conf 
-rw-r--r-- 1 postgres postgres 26898 Jul 21 20:00 /etc/postgresql/12/main/postgresql.conf
data_directory = '/var/lib/postgresql/12/main'          # use data in another directory

postgres@postgres-dpt-test:~$ /usr/lib/postgresql/15/bin/initdb -D /data/pgsql/15/main
/usr/lib/postgresql/15/bin/pg_ctl -D /data/pgsql/15/main -l logfile start
GCP 1P ->https://console.cloud.google.com/netapp/volumes?cloudshell=false&project=cvs-pm-host-1p
GCP 3P ->https://console.cloud.google.com/apis/library/cloudvolumesgcp-api.netapp.com?project=cloud-heroes 

https://stackoverflow.com/questions/31645550/postgresql-why-psql-cant-connect-to-server —> to debug if multiple versions are running.

/usr/lib/postgresql/15/bin/postgres -D /var/lib/postgresql/15/main -c config_file=/etc/postgresql/15/main/postgresql.conf
postgres@dpt-pg-cv-ontap-test-sj:~$ cat /var/lib/postgresql/15/main/postmaster.opts
/usr/lib/postgresql/15/bin/postgres "-D" "/var/lib/postgresql/15/main" "-c" "config_file=/etc/postgresql/15/main/postgresql.conf"
postgres@dpt-pg-cv-ontap-test-sj:~$ 
