Améliorer sa délivrabilité
==========================

Nous donnons quelques conseils pour la composition de vos mailings sur la page : :doc:`template_mailing`.

Vous devez également configurer vos DNS pour permettre d'authentifier vos mailings. 

* Déclarer Akemail comme emetteur autorisé (`SPF`_ = Sender Prolicy Framework)
* Authentifier votre domaine (signature `DKIM`_ = Domain Keys Indentified Mail)
* Définir une politique globale de traitement des erreurs (`DMARC`_ = Domain-based Message Authentication, Reporting, and Conformance)

Tous ces éléments doivent se paramétrer depuis le panneau d'administration de votre domaine
ou l'éditeur de zone.

Configuration du SPF
--------------------

Si vous utilisez déjà la protection `SPF`_ pour protéger vos mails d'entreprise, 
vous devez rajouter les serveurs d'akemail dans votre enregistrement SPF:

    **include:akemail.fr**

Si vous n'avez pas encore configuré de `SPF`_, vous devez créer un enregistrement TXT de cette forme :

    "v=spf1 mx **include:akemail.fr** -all"

Configuration du DKIM
---------------------

Créez un enregistrement CNAME pour **akemail._domainkey** avec cette valeur : 

    dkim.akemail.fr.

Configuration du DMARC
----------------------

Créez un enregistrement TXT pour **dmarc** avec cette valeur : 

    "v=DMARC1; p=reject; adkim=s; aspf=s"

Cela va demander au destinataire de rejeter les emails si `SPF`_ ou `DKIM`_ ne sont pas valides.

Vous pouvez bien évidemment adapter ces règles à vos besoins, y compris permettre 
la récupération des rapports d'erreurs. Mais il est important de définir des règles 
via cet enregistrement `DMARC`_.

.. _SPF: https://fr.wikipedia.org/wiki/Sender_Policy_Framework
.. _DKIM: https://fr.wikipedia.org/wiki/DomainKeys_Identified_Mail
.. _DMARC: https://fr.wikipedia.org/wiki/DMARC
