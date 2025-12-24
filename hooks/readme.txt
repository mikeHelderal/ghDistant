Installation du hook pre-commit (Git Bash / Linux / macOS)

1) Depuis la racine du dépôt :
   mkdir -p .git/hooks
   cp hooks/pre-commit .git/hooks/pre-commit
   chmod +x .git/hooks/pre-commit

2) Effet :
   Lors d'un commit, le hook demande si l'on veut générer un fichier de suivi.
   Si 'y' : crée/maj suivi/commitInfo.txt contenant "commit vérifié le <date heure>"
   et ajoute automatiquement ce fichier au commit.
