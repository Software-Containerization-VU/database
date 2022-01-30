# database

Create the config Map
### `kubectl apply -f postgres-config.yaml`

Create the Secret
### `kubectl apply -f postgres-secret.yaml`

Create the Statefulset
### `kubectl apply -f postgres-statefulset.yaml`

Create NodePort Service
### `kubectl apply -f postgres-nodeport.yaml`

Check that Postgresql was corretly set up on the NodePort 30001
### `psql -h localhost -U postgresadmin --password -p 30001 inventory_pg`
List the databases and exit
### `\l`
### `\q`