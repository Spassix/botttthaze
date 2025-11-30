# Bot Telegram - SPEED NICE

Bot Telegram pour SPEED NICE avec menu interactif et fonctionnalités de diffusion.

## Installation

1. Installez les dépendances :
```bash
pip install -r requirements.txt
```

2. Créez un fichier `.env` à partir du modèle `.env.example` et remplissez-le avec vos informations :
```bash
cp .env.example .env
```

3. Créez un fichier `.env` avec les variables suivantes :
   - `BOT_TOKEN` : Token de votre bot Telegram
   - `ADMIN_ID` : Votre ID Telegram (pour la commande /broadcast)
   - `MINI_APP_URL` : URL de la Mini App (Potato) - ex: https://dym168.org/Speednice_06
   - `TELEGRAM_URL` : Lien Telegram - ex: https://t.me/+s9VnDuQiBFY1ZmQ0
   - `CANAL_SECOURS_URL` : Lien Telegram secours - ex: https://t.me/+gree7fAvNwM1OTc0
   - `WHATSAPP_URL` : Lien WhatsApp - ex: https://wa.me/33758855772

4. Ajoutez l'image du logo dans le dossier (nommée `speednice_logo.png`)

5. **IMPORTANT** : Si vous déployez sur Render, arrêtez le bot local pour éviter les conflits.

6. Lancez le bot :
```bash
python bot.py
```

**Note pour le déploiement sur Render :**
- Le bot utilise automatiquement les webhooks sur Render
- Assurez-vous que le bot local est arrêté avant de déployer sur Render
- Les variables d'environnement doivent être configurées dans les paramètres Render

## Fonctionnalités

- **Menu interactif** avec boutons pour :
  - Mini App (Potato)
  - Lien Telegram
  - Canal Secours
  - Lien WhatsApp

- **Commande /start** : Affiche le menu principal avec l'image du logo

- **Commande /broadcast** : Permet à l'admin de diffuser des messages

## Configuration

Le token du bot et les URLs sont configurés dans le fichier `bot.py`.

