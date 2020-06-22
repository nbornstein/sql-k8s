# sql-k8s

Requires a kubernetes secret for the SA password, like so:

    kubectl create secret generic mssql --from-literal=SA_PASSWORD="p@55w0rd!!!"
