# ⭐ LAB-18 | ViewModel-LiveData-CounterApp
Une application Android démontrant l’utilisation de l’architecture moderne Android avec **ViewModel** et **LiveData** afin de gérer un compteur persistant lors des rotations d’écran et des changements de configuration.
---
## ✨ Fonctionnalités
- ➕ **Incrémentation du compteur**
- ➖ **Décrémentation du compteur**
- 🔄 **Réinitialisation instantanée**
- ♻️ **Persistance des données** après rotation d’écran
- 👀 **Mise à jour automatique de l’UI** grâce à LiveData
- 🧠 **Séparation logique / interface** avec ViewModel
- ⚡ **Architecture lifecycle-aware** moderne Android
---
## 🛠️ Stack technique
| Composant | Technologie |
|---|---|
| Langage | Java |
| UI | XML Layouts |
| Architecture | MVVM |
| State Management | ViewModel |
| Data Observation | LiveData |
| Lifecycle | AndroidX Lifecycle |
---
## 📁 Architecture du projet
```bash
com.example.viewmodellivedatademoenrichi
├── MainActivity.java          # Interface utilisateur
├── CounterViewModel.java      # Gestion logique et état du compteur
└── activity_main.xml          # Layout principal
```
---
## 📦 Dépendances
```gradle
dependencies {
    def lifecycle_version = "2.8.7"
    implementation("androidx.lifecycle:lifecycle-viewmodel:$lifecycle_version")
    implementation("androidx.lifecycle:lifecycle-livedata:$lifecycle_version")
}
```
---
## 🧠 Concepts Android abordés
- 📌 ViewModelProvider
- 📌 MutableLiveData
- 📌 Observer Pattern
- 📌 Lifecycle-Aware Components
- 📌 MVVM Architecture
- 📌 Gestion des changements de configuration
---
## 🔄 Fonctionnement
1. L'utilisateur clique sur un bouton
2. Le ViewModel modifie la valeur du compteur
3. LiveData notifie automatiquement l'Observer
4. L'interface se met à jour sans manipulation directe
---
## 📱 Interface
- Grand affichage du compteur
- Trois boutons :
  - INCRÉMENTER
  - DÉCRÉMENTER
  - RÉINITIALISER
---
## Demo
- Partie 01:
https://github.com/user-attachments/assets/a8585347-22be-459f-97c8-3cd9ebf7c423
- Partie 02:
https://github.com/user-attachments/assets/296349d4-a319-46de-9a91-2408a0e03ebd
---
## 🎯 Objectif pédagogique
Ce laboratoire montre pourquoi les composants modernes Android comme ViewModel et LiveData sont préférables à :
- `onSaveInstanceState()`
- variables d’instance classiques
- gestion manuelle des rotations
---
## 👨‍💻 Auteur
**Mourad EL OUATIK** | Réalisé dans le cadre du **Lab 18 Android** | Programmation & Securite des Applications Mobile
