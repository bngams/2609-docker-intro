# selectionner l'env. de base
FROM node:24-alpine3.24

# récupérer les fichiers
COPY package.json /app/
COPY index.js /app/

# executer npm install
RUN cd /app && npm install

# ENTYPOINT...
# lancement node index.js
CMD ["node", "/app/index.js"]
# CMD node index.js
