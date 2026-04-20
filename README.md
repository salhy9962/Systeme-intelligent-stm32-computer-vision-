Smart Security System ( STM32 + Keypad + Radar + Computer Vision) 
Description

Ce projet présente un système de surveillance intelligent combinant systèmes embarqués (STM32) et vision par ordinateur pour sécuriser l’accès à une porte.

Le système permet de contrôler l’accès via un clavier matriciel (keypad), de détecter la présence avec un radar à ultrasons (HC-SR04 + servo moteur), et d’assurer une surveillance avancée avec reconnaissance faciale via une caméra PC.
Répartition du travail

 Mon rôle :
Programmation STM32
Implémentation FreeRTOS
Gestion du keypad
Radar (ultrason + servo)
Contrôle de la porte

Mon Collègue :
Computer Vision
Capture d’image
Envoi d’email

Fonctionnement du système
🔹 1. Authentification par mot de passe
L’utilisateur saisit un mot de passe via le keypad
✔️ Si le mot de passe est correct :
La porte s’ouvre automatiquement via un servo moteur
❌ Si le mot de passe est incorrect :
Le système incrémente un compteur d’erreurs
🔹 2. Sécurité avancée (Computer Vision)
Après 3 tentatives incorrectes :
Activation de la caméra du PC
Capture d’une image du visage
Envoi automatique par email (alerte de sécurité)
🔹 3. Détection de présence (Radar)
Utilisation d’un capteur ultrason + servo moteur
Scan de la zone pour :
détecter une présence devant la porte
améliorer la sécurité du système

Fonctionnalités
🔐 Système d’authentification sécurisé (mot de passe)
🚪 Ouverture automatique de porte (servo moteur)
📡 Détection de présence (radar ultrason)
🧠 Intégration Computer Vision
📧 Envoi d’alertes par email avec capture d’image
⚙️ Gestion multitâche avec FreeRTOS
🛠️ Technologies utilisées
🔹 Embedded
STM32 (FreeRTOS CMSIS v2)
Keypad 4x4
Capteur ultrason (HC-SR04)
Servo moteurs
🔹 Software
C / STM32CubeIDE
FreeRTOS (gestion des tâches)
🔹 Computer Vision
Python / OpenCV (caméra PC)
