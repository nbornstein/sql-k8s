# sql-k8s

Manifest to deploy SQL Server on a kubernetes cluster. Creates a PersistentVolumeClaim on cinder storage, and exposes the SQL server on port 80 because port filtering won't allow the standard 1433.

Requires a kubernetes secret for the SA password, like so:

    kubectl create secret generic mssql --from-literal=SA_PASSWORD="p@55w0rd!!!"

