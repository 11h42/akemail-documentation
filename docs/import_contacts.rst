.. _ref-import_contacts:

=====================
Importer des contacts
=====================

Importer des contacts
---------------------

Vous pouvez créer un contact dans `Akemail`_ en cliquant sur le bouton **importer des contacts** depuis le Dashboard:

.. figure::  _static/images/bookmark.png
   :align:   center

ou depuis la page **contacts** accessible depuis le menu principal:

.. figure::  _static/images/submenu.png
   :align:   center

L'import de contact se fait en trois étapes:

 *  La selection d'un fichier **CSV**
 *  Le renseignement des en-têtes
 *  La destination des contacts fraichement créés

Un fichier **CSV** (Comma-separated values) est un format informatique ouvert représentant des données tabulaires sous
forme de valeurs séparées par des virgules.
Excel, Libre Office, Google Document, etc... Tous ces logiciels permettent d'exporter vos données au format CSV.

Les en-têtes correspondent aux noms des colonnes de votre fichier **CSV**. Ils deviendront des champs personnalisés
pour chaque contact (comme décrits plus haut).

Si durant cette étape, le nombre de colonnes affichées ne correspond pas au nombre de colonnes souhaitées, alors votre
fichier **CSV** n'est pas valide. Arrétez vous là, modifier votre fichier **CSV** et reprenez un import à zéro.

.. figure::  _static/images/headers.png
   :align:   center

Terminez votre import en selectionnant la destination de vos contacts puis cliquez sur le bouton
**Importer vos contacts**

Imports en cours/terminés
-------------------------

Un import de contacts est une tache qui peut prendre du temps. Cette tâche est effectuée en tâche de fond, vous pouvez
pendant un import utiliser Akemail.

La liste des imports que vous avez effectués est disponible dans Akemail depuis le sous-menu dans la page **contacts**

.. figure::  _static/images/imports.png
   :align:   center

Un import passe de l'état EN PREPARATION à l'état PRÊT, puis EN COURS, puis ERREUR ou TERMINÉ

Un rapport d'import est disponible en cliquant sur **rapport**.

.. figure::  _static/images/rapport_import.png
   :align:   center

Il donne des informations sur les erreurs de votre fichier: les doublons, les emails invalides, les lignes ignorées et
précise pour chacune des erreurs la ligne à laquelle l'erreur s'est produite.

 *  Un email n'est inséré qu'une seule fois
 *  Un email invalide n'est pas inséré
 *  Une ligne sans email est ignorée (comme l'entête de votre fichier si elle se trouve au debut de votre fichier **CSV**)

Un import de contacts, peut rester à l'état PRÊT quelques heures. Il correspond à un import de contacts pour lequel vous
avez importé un fichier puis abandonné l'opération.

.. _Akemail: https://akemail.fr/
