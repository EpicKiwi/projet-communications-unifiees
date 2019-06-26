# Composants

## Containers

* **Orchestrateur** : Rancher
	* Déploiement : Terraform
* **VoIP** et **visioconference**
	* IPBX : Asterisk
		* Persistance des fichiers CSV
	* Client : Linphone
* **Pad** : Etherpad
	* Vérifier la nécessité d'une BDD ou d'une persistance
* **BDD** : ElasticSearch
	* Persistance des données
* **Messagerie**, **contacts** et **agenda** : 
	* SMTP(S) : Postfix
		* Persistance des messages en cours d'envoi
	* IMAP(S) : Dovecot
		* Persistance des messages stockés (Grosse quantité)
	* CalDAV, CardDAV : Radicale
		* Persistance des calendriers et contacts
	* Webmail : Sogo
* LDAP : OpenLDAP
	* Persistance de l'annuaire
* **Gestionnaire de fichier**
	* WebApp & WebDAV : NextCloud
* **Traitement de texte**, **tableur**
	* WebApp : OnlyOffice
		* Connexion au serveur de fichiers WebDAV
* **Wiki** : Gitit
	* Persistance du wiki
* **Forum** : Discourse
	* persistance des posts
* **Chat** : Rocket.chat
	* persistance des conversations
* **Réseau social** : Mastodon
	* persistance des toots
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