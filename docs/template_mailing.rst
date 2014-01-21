.. _ref-template_mailing:

=====================
Template d'un mailing
=====================

Le template d'un mailing est la partie la plus difficile dans la création d'un mailing.

Qu'est ce qu'un template ?
--------------------------
Le template d'un mailing est le contenu de votre mailing. Il correspond au corp du mail que vous allez envoyer à tous
vos clients. Un mauvais template peut par exemple faire baisser très fortement la délivrabilité d'un mailing. Un mauvais
template peut vous envoyer dans la boite spam de vos clients.

Qu'est ce qu'un bon template pour un mailing ?
----------------------------------------------

C'est une question difficile, néanmoins voici quelques éléments de réponse:

 * un bon template s'adapte à la taille de l'écran de vos clients. Un email ne doit pas faire la même taille sur un écran de téléphone ou un écran d'ordinateur. On parle ici d'email responsive.
 * un bon template n'est pas constitué que d'une seule image. Beaucoup de client mail, ne charge pas les images. C'est un système anti-spam historique qui est toujours d'actualité aujourd'hui.
 * un bon template est personnalisé, ajouter des contacts avec des champs personnalisés, puis personnalisez vos mailings avec (exemple: Bonjour {{ prenom }})
 * un bon template est pertinent. Si beaucoup de vos clients, considèrent comme spam votre mailing, vous allez dégrader votre adresse email. Vous risquez la prochaine fois d'être considéré comme du spam directement.

Personalisation d'un mailing
----------------------------

Lorsque vous importez vos contacts, vous pouvez spécifier le contenu des entêtes de vos colonnes.
Un contact, en fonction du nom des entêtes, se voit attribuer un champ personnalisé correspondant.

.. figure::  _static/images/custom_fields.png
   :align:   center

Vous pouvez dans vos emails utiliser ses champs personnalisés pour personnaliser vos emails. Par exemple si vous avez
un contact avec le champ personnalisé **entreprise** qui correspond à son entreprise.

Vous pouvez dans votre mailing rajouter les informations personnalisées entourées de doubles accolades


    Nous remercions {{ entreprise }} pour...


qui sera remplacé dans l'email par


    Nous remercions Akemail pour...


Lien de désinscription
----------------------


**/!\\ Akemail rend obligatoire le lien de désinscription. Ce dernier doit figurer dans votre mailing.**
Nous vérifions qu'un lien est présent dans votre mailing avec la valeur personnalisée {{ UNSUBSCRIBE }}.


    <a href="{{ UNSUBSCRIBE }}">Me désinscrire</a>

Si cette information n'est pas présente, alors Akemail rajoute pour vous cette information à la fin de votre mailing.

    <a href="{{ UNSUBSCRIBE }}">Me désinscrire</a>

Ce qui est remplacé par un lien simple dans votre mailing.
