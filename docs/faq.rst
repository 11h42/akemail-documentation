.. _ref-faq:

====================
Questions fréquentes
====================

Pourquoi rajoutez vous automatiquement un lien de désinscription à la fin de mon mailing ?
------------------------------------------------------------------------------------------

Le lien de désinscription permet à votre mailing de ne pas être considéré comme un spam. La plus part des fournisseurs
d'adresse email (Gmail, Yahoo, Outlook, AOL) considèrent souvent un mailing comme spam s'il ne possède pas de lien de désinscription.

Plus d'information: :doc:`template_mailing`


J'ai oublié mon mot de passe, comment puis-je le récupérer ?
------------------------------------------------------------

La fonctionnalité qui permet de récupérer son mot de passe, n'est pas encore réalisée. Pour l'instant, vous pouvez
nous contacter par email à support@akemail.fr pour nous demander un nouveau mot de passe.


J'ai besoin d'un connecteur pour envoyer mes mailings depuis mon logiciel d'entreprise, Akemail peut-il m'aider ?
-----------------------------------------------------------------------------------------------------------------

Akemail peut développer des connecteurs pour vos logiciels d'entreprise. Sur la base d'un cahier des charges,
nous développons avec vous un connecteur pour gérer vos mailings d'entreprise. Plus de serveurs mails à gérer et à
mettre à jour, plus d'administrateur système pour configurer vos serveurs de mail.
Nous créons des connecteurs pour SAP, OpenERP, applications mobiles, application web, etc.

Vous voulez plus d'informations ? Envoyez nous un email à contact@akemail.fr


Comment puis-je augmenter ma délivrabilité ?
--------------------------------------------
Si vous utilisez la protection `SPF`_ pour protéger vos mails d'entreprise, vous pouvez rajouter les serveurs d'email d'akemail dans votre SPF:

**include:akemail.fr**

Votre enregistrement dans vos DNS doit ressembler à :

**v=spf1 mx include:mon-entreprise.com include:akemail.fr ~all**

.. _SPF: http://fr.wikipedia.org/wiki/Sender_Policy_Framework