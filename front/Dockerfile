# Utilise une image Node.js comme base
FROM node:14-alpine

# Définit le répertoire de travail dans le conteneur
WORKDIR /usr/src/app

# Copie le package.json et le package-lock.json dans le conteneur
COPY package*.json ./

# Installe les dépendances
RUN npm install

# Copie les fichiers du projet dans le conteneur
COPY . .

# Construit l'application React pour la production
RUN npm run build

# Expose le port 80 sur le conteneur
EXPOSE 80

# Démarre l'application lors du lancement du conteneur
CMD ["npm", "start"]
