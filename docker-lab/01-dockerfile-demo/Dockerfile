# UN ENV. CONTENEURISE pour exec. PYTHON

# =====================================
# PISTE 1: je pars d'une base system LINUX et j'installe python
# =====================================
# FROM alpine:3.24

# installer python ...
# 2 pistes avec apk ou DDL binaries
#RUN apk update -y && apk add python3 -y
# d'autres commandes

# =====================================
# PISTE 2 : je pars d'une base ptyhon (linux based...)
# =====================================
FROM python:3.12.14-alpine3.24


# =====================================
# COMMUN : config app
# =====================================

# téléverser / copier le app.py dans l'image
# scp ./app.py image:/app
# COPY SRC(form local filesystem) DEST(dans l'image) 
COPY app.py /myapp/

# configurer l'image pour lancer app.py au démarrage du container
CMD ["python3", "/myapp/app.py"]