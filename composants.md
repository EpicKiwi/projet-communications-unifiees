# Composants

## Containers

* **Orchestrateur** : Rancher
	* Déploiement : Terraform
* **VoIP** et **visioconference**
	* IPBX : Asterisk
		* Persistance des fichiers CSV
		* Authetification LDAP
	* Client : Linphone
* **Pad** : Etherpad
	* BDD Mysql
* **BDD** : ElasticSearch
	* Persistance des données
	* Authetification LDAP
* **Messagerie**, **contacts** et **agenda** : 
	* SMTP(S) : Postfix
		* Persistance des messages en cours d'envoi
		* Authetification LDAP
	* IMAP(S) : Dovecot
		* Persistance des messages stockés (Grosse quantité)
		* Authetification LDAP
	* CalDAV, CardDAV : Radicale
		* Persistance des calendriers et contacts
		* A verifier (Sogo sert peut etre de serveur)
	* Webmail : Sogo
		* Basde de données
		* Authetification LDAP
* LDAP : OpenLDAP
	* Persistance de l'annuaire
* **Gestionnaire de fichier**
	* WebApp & WebDAV : NextCloud
	* Authetification LDAP
* **Traitement de texte**, **tableur**
	* WebApp : OnlyOffice
		* Connexion au serveur de fichiers WebDAV
		* Authetification LDAP
* **Wiki** : Gitit
	* Persistance du wiki
	* Authetification LDAP
* **Forum** : Discourse
	* persistance des posts
	* Authetification LDAP
* **Chat** : Rocket.chat
	* persistance des conversations
	* Authetification LDAP
* **Réseau social** : Mastodon
	* persistance des toots
	* Authetification LDAP
* **Reverse proxy** et **Load balancing**
	* Serveur : Nginx
	* Certificat : Let's encrypt

## Hardware

* **LY0201** Master-Emerald
	* 3 VCPU
	* 8 Go RAM
	* 100 Go HDD
* **LY0202** Replica-Sapphire
	* 2 VCPU
	* 5 Go RAM
	* 70 Go HDD
* **LY0203** Replica-Ruby
	* 2 VCPU
	* 5 Go RAM
	* 70 Go HDD
* **TOTAL**
	* 7 VCPU
	* 18 Go de RAM
	* 240 Go de HDD