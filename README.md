# IA_Local_Benchmark
Permet de tester des modèles d'IA local sur différents hardware

--------------------------------------------------------------------------------
1. STRUCTURE DU PROJET PORTABLE
--------------------------------------------------------------------------------
  ├── start_cockpit.sh          -> Script principal (Auto-installation + Lancement)
  ├── export_portable.sh        -> Génère l'archive portable IA_Benchmark_Portable.tar.gz
  ├── requirements.txt          -> Liste des dépendances Python installées automatiquement
  ├── GUIDE_DEPLOIEMENT.txt     -> Ce guide d'instructions et de commandes
  └── app/                      -> Dossier contenant le code source (100% modifiable)
      ├── main.py               -> Serveur Backend FastAPI, WebSocket, Télémétrie GPU & vLLM
      ├── templates/
      │   └── index.html        -> Interface graphique HTML (TailwindCSS + Chart.js)
      ├── static/
      │   └── app.js            -> Logique Frontend, Graphiques temps réel & Export CSV
      └── data/
          └── benchmarks_history.json -> Historique sauvegardé des tests et courbes
