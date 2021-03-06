# Éditeur de clé de dictionnaire rehaussé Sigmund

[![Build status](https://sigmundftw.visualstudio.com/EnhancedDictionaryEditor/_apis/build/status/EnhancedDictionaryEditor%20Build%20pipeline)](https://sigmundftw.visualstudio.com/EnhancedDictionaryEditor/_build/latest?definitionId=78)

Permet de 
- Voir la liste des clés                    (1.0.0)
- Créer des clés                            (1.0.0)
- Modifier des clés                         (1.0.0)
- Supprimer des clés                        (1.0.0)
- Rechercher par identifiant ou par valeur  (1.0.0)
- Importer et exporter la liste des clés    (1.1.0)
- Bouton de traduction automatique          (1.2.0)

## Bouton de traduction automatique 

La traduction automatique vous permet d'implémenter une classe qui sera utilisée pour traduire les textes des clés.
Pour ce faire, définissez une classe implémentant l'interface "ITranslator" et configurez l'application au démarrage pour en faire utilisation.

```
DictionaryKeyTranslatorProvider.SetTranslator(new Translator());
```

## Pour installer dans votre projet Umbraco

```
Install-Package EnhancedDictionaryEditor
```

## Installation développeur

- Clonez le repository
- Ouvrez le projet dans Visual Studio 2017
- Installez le package nuget: `UmbracoCms`
- Copiez le contenu des fichiers situés dans le dossier Sigmund.EnhancedDictionaryEditor\Transforms\config dans les fichiers de configuration d'umbraco.
- Faites un build du projet.
- Configurez IIS pour le projet web Sigmund.EnhancedDictionaryEditor
- Accédez à `http://{adresse_dans_iis}/umbraco
- Installez la base de donnée à l'aide de l'assistant.
- Donnez accès à votre groupe d'utilisateur "Administrators" à la section du plugin.
- Accédez à l'interface du plugin dans la barre de gauche.


