# Politique de confidentialité

**Dernière mise à jour : 6 octobre 2026**

[English version](privacy.html) · [Conditions d'utilisation](conditions.html)

---

## 1. Qui traite vos données

**Maxime Bouchard**, personne physique, éditeur de l'application KiFéKoi.

Contact pour toute question ou pour exercer vos droits :
[mbouchard.dev@gmail.com](mailto:mbouchard.dev@gmail.com)

---

## 2. Le point le plus important : deux modes, deux réponses

KiFéKoi fonctionne de deux façons, et **le choix vous appartient**. Il se trouve
dans *Paramètres › Stockage du foyer*.

### Mode « Sur cet appareil » (par défaut)

**Aucune donnée ne quitte votre téléphone.** Pas de compte en ligne, pas de
serveur, pas de sauvegarde distante. Les tâches, l'historique, les réponses de
check-in et les scores restent dans le stockage de l'application.

Dans ce mode, cette politique n'a presque rien à décrire : il n'y a pas de
traitement de notre part, parce qu'il n'y a pas de transmission. La seule
conséquence est qu'un foyer perdu avec le téléphone est perdu définitivement.

C'est le mode **actif par défaut**. L'application ne bascule jamais toute seule.

### Mode « Partagé »

Vous choisissez ce mode pour partager un foyer entre plusieurs appareils. Les
données décrites ci-dessous sont alors hébergées sur un serveur.

---

## 3. Données traitées en mode partagé

| Donnée | Pourquoi | Base légale (RGPD) |
|---|---|---|
| **Prénom** saisi à l'onboarding | Identifier qui porte quoi dans le foyer | Exécution du contrat (art. 6.1.b) |
| **Identifiant de compte anonyme** | Rattacher votre appareil à votre place dans le foyer | Exécution du contrat |
| **Contenu du foyer** : tâches, notes, échéances, attributions, historique | Le service lui-même | Exécution du contrat |
| **Réponses de check-in** hebdomadaire | Comparer le ressenti au calcul | Exécution du contrat |
| **Jeton de notification (APNs)** | Vous prévenir quand l'autre personne vous confie une tâche | **Consentement** (art. 6.1.a) |
| **Identifiant de transaction d'abonnement** | Vérifier auprès d'Apple que l'abonnement est actif | Exécution du contrat |

### Sur le compte « anonyme »

Le compte est créé sans e-mail ni mot de passe : l'application demande un prénom,
rien d'autre. L'identifiant obtenu ne contient aucune information sur vous et
n'est relié à aucun annuaire.

Une conséquence à connaître : **ce compte vit dans le trousseau de votre
appareil**. Le perdre, c'est perdre l'accès au foyer partagé, sans moyen de
récupération.

### Sur les réponses de check-in

Ce sont les données les plus personnelles de l'application — on y écrit des
choses comme « j'ai eu l'impression d'être seul·e à y penser ». Elles ne sont
lisibles que par les membres de votre foyer. Cette restriction n'est pas une
promesse de notre part : elle est imposée par la base de données elle-même
(*Row Level Security*), indépendamment du code de l'application.

### Sur le jeton de notification

Il n'est transmis que si vous activez les notifications distantes, et il est
supprimé du serveur dès que vous les désactivez. C'est le seul traitement fondé
sur votre consentement, et il est donc révocable à tout moment, sans
conséquence sur le reste du service.

---

## 4. Ce que nous ne faisons pas

- **Aucune publicité.** L'application n'embarque aucune régie.
- **Aucun suivi.** Pas de SDK analytique, pas d'identifiant publicitaire, pas de
  mesure d'audience, pas de suivi d'une application à l'autre. Le manifeste de
  confidentialité livré avec l'app déclare `NSPrivacyTracking: false`.
- **Aucune revente ni partage commercial.** Vos données ne sont transmises à
  personne d'autre que les sous-traitants techniques listés ci-dessous.
- **Aucun profilage, aucune décision automatisée** produisant des effets
  juridiques à votre égard. Les scores d'équilibre sont un calcul affiché, pas
  une décision.
- **Aucune lecture de votre part.** L'éditeur n'accède pas au contenu des foyers.

---

## 5. Sous-traitants

| Prestataire | Rôle | Localisation |
|---|---|---|
| **Supabase** | Hébergement de la base et des fonctions serveur | **Irlande (Union européenne)** |
| **Apple** | Notifications (APNs), achats et abonnements | Selon la politique d'Apple |

**Le contenu de votre foyer ne quitte pas l'Union européenne.** La base de
données et les fonctions serveur sont hébergées en Irlande ; il n'y a donc aucun
transfert hors UE à encadrer pour ces données.

Deux réserves, dites franchement : les notifications transitent par les serveurs
d'Apple (APNs) et la vérification d'abonnement interroge l'App Store, deux
traitements qui suivent la politique d'Apple et non la nôtre. Ils ne portent que
sur un jeton d'appareil et un identifiant de transaction — jamais sur le contenu
de votre foyer.

Apple est par ailleurs l'intermédiaire de paiement des abonnements : **nous ne
recevons ni ne voyons aucune donnée bancaire**.

---

## 6. Durées de conservation

- **Contenu du foyer** : conservé tant que le foyer existe. Supprimé
  immédiatement et définitivement lorsque le dernier membre quitte le foyer ou
  le supprime.
- **Compte** : supprimé immédiatement à votre demande (voir §8).
- **Jeton de notification** : supprimé dès la désactivation des notifications,
  ou automatiquement lorsque Apple nous signale que l'application a été
  désinstallée.
- **Trace d'abonnement** : conservée tant que l'abonnement court, puis marquée
  comme révoquée afin de pouvoir répondre à « pourquoi est-ce redevenu
  gratuit ? ».

---

## 7. Vos droits

Vous disposez des droits d'accès, de rectification, d'effacement, de limitation,
d'opposition et de portabilité prévus par le RGPD, ainsi que du droit de retirer
votre consentement aux notifications à tout moment.

Deux de ces droits s'exercent **directement dans l'application**, sans avoir à
écrire à qui que ce soit :

- **Rectification** : *Paramètres › Membres* pour le prénom.
- **Effacement** : *Paramètres › Supprimer mon compte* (voir §8).

Pour les autres, écrivez à l'adresse du §1. Vous pouvez également introduire une
réclamation auprès de la [CNIL](https://www.cnil.fr).

---

## 8. Supprimer votre compte

*Paramètres › Supprimer mon compte*, dans l'application.

Ce que cela fait exactement :

1. Votre place dans le foyer est retirée, avec votre prénom.
2. Votre compte est supprimé du serveur d'authentification.
3. Vos jetons de notification sont supprimés.
4. **Si vous étiez le dernier membre**, le foyer et tout son contenu sont
   supprimés avec vous.

Ce que cela ne fait **pas** : si d'autres personnes partagent le foyer, le foyer
et son historique leur restent. Nous ne détruisons pas les données d'un tiers
parce que vous partez — mais les occurrences que vous portiez cessent de vous
être attribuées.

L'opération est immédiate et irréversible.

---

## 9. Sécurité

- Toutes les communications passent par **HTTPS**.
- Le cloisonnement entre foyers est imposé par la base de données
  (*Row Level Security*), et non par le code de l'application. Une erreur de
  programmation côté app ne peut donc pas exposer le foyer de quelqu'un d'autre.
- La clé d'administration du serveur n'existe que côté serveur. Elle n'est
  **jamais** embarquée dans l'application.

Aucun système n'est inviolable, et nous ne prétendons pas le contraire.

---

## 10. Enfants

KiFéKoi s'adresse à des adultes vivant en foyer. L'application n'est pas destinée
aux mineurs de moins de 15 ans et ne leur propose pas de créer un compte.

Un foyer peut toutefois comporter des membres identifiés comme « enfant ». Dans
ce cas, **seul leur prénom est enregistré, par un adulte du foyer, et ils n'ont
ni compte ni accès à l'application**. Il revient à l'adulte qui les ajoute de
s'assurer que c'est approprié.

---

## 11. Modifications

Toute modification sera publiée sur cette page avec une nouvelle date de mise à
jour. Un changement substantiel sera signalé dans l'application.
