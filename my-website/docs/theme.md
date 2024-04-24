# Configuration du thème

## Mode de couleur

Le thème classic fournit par défaut la prise en charge du mode clair et sombre, avec un commutateur dans la barre de navigation pour l'utilisateur.

Il est possible de personnaliser le support du mode de couleur dans l'objet colorMode.


Nom	Type :                      Par défaut :	                Description :

defaultMode	'light'          | 'dark'	'light'	              Le mode de couleur lorsque l'utilisateur visite le  ->                                                            site pour la première fois.
disableSwitch	                boolean	false	              Masque l'interrupteur dans la barre de navigation. ->                                                            Utile si vous voulez prendre en charge un mode de ->                                                            couleur unique.
respectPrefersColorScheme	    boolean	false	              Si vous voulez utiliser la requête media-query       ->                                                            prefers-color-scheme, en utilisant les préférences du ->                                                            système utilisateur, au lieu du defaultMode codé en ->                                                            dur.


Exemple de configuration :
```
export default {
  themeConfig: {
    colorMode: {
      defaultMode: 'light',
      disableSwitch: false,
      respectPrefersColorScheme: false,
    },
  },
};
```