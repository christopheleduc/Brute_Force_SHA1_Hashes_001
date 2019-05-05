# DiscoPass - Hash et compare un mot de passe à partir d'un fichier texte.

# "DiscoPass.py" est largement commenté !

Un petit programme en Python qui "Hash" un mot de passe avec SHA1 (mais ce pourrait être MD5), récupère une liste de mots de passe connues, "Hash" chacun des mots de passe, et procède à une comparaison.

Il y a 2 méthodes, la première utilise un fichier texte local (facile à maintenir à jour), et l'autre récupère un fichier texte distant (internet).

On importe "urlopen", "hashlib" et "time". Donc vérifiez que ces 3 dépendances sont présentes en cas d'erreur...

Il est possible d'augmenter la sécurité des mots de passe en vérifiant qu'ils ne sont pas trop communs ou carrément déjà connues, ce qui fragilise grandement la sécurité.

Cet outil peut permettre de démontrer avec quel facilité il est facile de mettre en œuvre des techniques de brute-forcing...

Il y a 2 fichiers texte fournit:

1_mille_knows_password_1000.txt contient mille mots de passe.

1_million_knows_password_1000000.txt contient un million de mots de passe.

