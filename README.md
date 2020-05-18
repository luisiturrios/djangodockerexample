# Django Docker Example

A Django based project to explain how to set up fresh install of Django Celery Rabbitmq Postgres

## Docker services

### message-broker
rabbitmq 3.8.3 service expose port 5672

### database-server
postgres 12.3 service expose port 5432

### celery-beat
celery beat is a scheduler; It kicks off tasks at regular intervals, that are then executed by available worker nodes in the cluster.

### celery-worker
celery worker service

### wsgi-server
Uwsgi 12.3 app service expose port 3031

### web-server
Nginx service expose ports 80 and 443
