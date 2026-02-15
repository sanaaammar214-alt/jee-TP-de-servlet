# SanaPay - Application Fintech de Paiement

## 🎯 Description
SanaPay est une application fintech de paiement et de transfert d'argent offrant un portefeuille électronique sécurisé, des paiements digitaux, des transferts instantanés et des services financiers adaptés aux particuliers et aux entreprises.

## 🏗️ Architecture du Projet

### Backend - NestJS
```
backend/
├── src/
│   ├── auth/              # Module d'authentification (JWT, 2FA)
│   ├── users/             # Gestion des utilisateurs
│   ├── wallets/           # Gestion des portefeuilles électroniques
│   ├── transactions/      # Gestion des transactions et transferts
│   ├── payments/          # Traitement des paiements
│   ├── notifications/     # Service de notifications
│   ├── common/            # Guards, interceptors, decorators
│   └── config/            # Configuration (DB, JWT, etc.)
```

### Frontend - MVC Pattern
```
frontend/
├── public/
│   ├── css/              # Styles CSS
│   ├── js/
│   │   ├── models/       # Models (données et logique métier)
│   │   ├── views/        # Views (affichage et templates)
│   │   ├── controllers/  # Controllers (logique d'interaction)
│   │   └── services/     # Services API
│   └── assets/           # Images, fonts, etc.
└── index.html
```

## 🚀 Fonctionnalités Principales

### Pour les Particuliers
- ✅ Inscription et authentification sécurisée (JWT + 2FA)
- ✅ Portefeuille électronique personnel
- ✅ Transferts d'argent instantanés
- ✅ Paiements de factures
- ✅ Historique des transactions
- ✅ Notifications en temps réel

### Pour les Entreprises
- ✅ Compte professionnel
- ✅ Gestion multi-utilisateurs
- ✅ Paiements en masse
- ✅ Rapports et analytics
- ✅ API pour intégration

## 🔐 Sécurité
- Authentification JWT
- Chiffrement des données sensibles
- Validation des entrées
- Protection CSRF
- Rate limiting
- Logs d'audit

## 📋 Prérequis
- Node.js (v18+)
- npm ou yarn
- PostgreSQL ou MongoDB
- Git

## 🛠️ Installation

### Backend
```bash
cd backend
npm install
cp .env.example .env
# Configurer les variables d'environnement
npm run start:dev
```

### Frontend
```bash
cd frontend
# Ouvrir index.html avec un serveur local
# Recommandé: Live Server (VS Code) ou http-server
npx http-server public -p 3000
```

## 🌐 API Endpoints

### Authentication
- POST `/api/auth/register` - Inscription
- POST `/api/auth/login` - Connexion
- POST `/api/auth/logout` - Déconnexion
- POST `/api/auth/refresh` - Rafraîchir le token

### Wallets
- GET `/api/wallets/balance` - Consulter le solde
- POST `/api/wallets/deposit` - Dépôt d'argent
- POST `/api/wallets/withdraw` - Retrait d'argent

### Transactions
- POST `/api/transactions/transfer` - Effectuer un transfert
- GET `/api/transactions/history` - Historique des transactions
- GET `/api/transactions/:id` - Détails d'une transaction

### Payments
- POST `/api/payments/bill` - Payer une facture
- POST `/api/payments/merchant` - Paiement marchand

## 📱 Captures d'écran
(À ajouter)

## 🤝 Contribution
Les contributions sont les bienvenues !

## 📄 Licence
MIT

## 👥 Auteur
Votre Nom
