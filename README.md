# here we will not use postgress files will isntall postgress directly from bitmani repo

# used this cmd to isnall postgress from batmani
# <
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install postgres -n obserb-demo bitnami/postgresql \
  --set auth.username=postgres \
  --set auth.password=postgres \
  --set auth.database=mydb \
  --set primary.persistence.enabled=true \
  --set primary.persistence.size=1Gi
# >

this helm config repos will be used for below two springboot microserice project with postgress db for observbility test with prometheus, grafana and loki
https://github.com/file-krafter/webapp1-with-pg-p-g-lt.git


https://github.com/file-krafter/webapp2-with-pg-p-g-lt.git

