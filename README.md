# Projet React + Symfony

## Installation

### Frontend (React)
```bash
cd frontend
npm install
npm run dev
```

### Backend (Symfony)
```bash
cd backend
composer install
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate
php bin/console lexik:jwt:generate-keypair
symfony server:start
```

## Structure du projet

### Frontend
- `/src/components`: Composants React réutilisables
- `/src/pages`: Pages de l'application
- `/src/services`: Services pour les appels API
- `/src/store`: Gestion de l'état avec Zustand
- `/src/hooks`: Hooks personnalisés
- `/src/interfaces`: Types TypeScript

### Backend
- `/src/Controller`: Contrôleurs Symfony
- `/src/Entity`: Entités Doctrine
- `/src/Repository`: Repositories Doctrine
- `/src/Service`: Services métier
- `/config`: Fichiers de configuration

## Développement
- Frontend: http://localhost:5173
- Backend: http://localhost:8000