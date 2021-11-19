# Retour de la demande de qualification d'IPs du 3/11/2021 par SafeAMorty.c0o

Bonjour cher clients, clientes,
notre équipe d'analyses et de surveillance réseau vous rendent leur diagnostique au sujet des différentes Artefacts inhabituelles apparaîssant sur le réseaux de votre société de design digital. Nous commençons par détailler les riques de chaques adresses puis terminerons par des recommandations pour votre système.

## Artefects Pixels

### 1) 188.168.217.62
 	à la date du 6/11/2021 à 18h00
	
Cette Ip à un score VirusTotal de 0/71, elle apparaît en France dernièrement sous le nom de domaine designspartan.com.
c'est un serveur qui fonctionne dans un environement linux (debian) hébergé chez OVH.com.
subnet 188.165.208.0/20.

- Conclusion:
Cet artefact vient d'une source française, un serveur à roubais hébergé chez OVH,
suite a nos investigation il n'y as pas de raison de s'inquiéter au sujet de cette adresse.
elle ne présente aucun risque à cette date, si elle semble se manifester à maintes reprise sur vos systemes il est conseillé de la bloquer par sécurité
- Qualification de 188.168.217.62:
>Criticité faible. les informations découverte sur cette ip ne permettent pas de corréler des signes de menaces pour votre système.

### 2) 99.84.237.62
	à la dete du 06/11/2021 à 18h30
Cette IP à un score VirusTotal de 0/71, elle appraît aux USA dans l'état du Kansas sous des noms de domaine appartanant à DEVIANTART.COM. Cette IP est un serveur hébergé chez Amazon.com.
Elle est associé à 126 entités de malwares d'après threatminer.


Conclusion : Nous avons découvert que cette ip est présente dans des blocklists et présente une liste de 126 entités déchantillons de malwares. En ajoutant à cela le fait qu'il utilise de nombreux commptes Deviantart de particulier nous concluons que c'est une menace pour votre système.
- Qualification de 99.84.237.62:
> Criticité haute. les informations découvertes sur cette ip permettent d'assurer la criticité de cette IP. Elle semble usurper l'identité d'artistes de devaintart.com et pourrais répendre de nombreux malwares. Cette menace ne peux être prise à la légère.

### 3) 103.219.112.88
	à la date du 8/11/2021 à 14h00
Cette ip à un score VirusTotal de 6/91, Elle apparaît en Indonésie. Elle présente de nombreux signes alarmants sur nos outils d'OSINT 
alientvault :
* 32 tags ( comme tpot19 honeypot bruteforce ou botnet, etc ...)
* 61 port ouvert (ce qui n'est pas anodin lorqu'on le met en lien avec les tags précédents)
* score spyse 0/100 ce qui est une preuve critique de sécurité

Conclusion :La correlation entre le score virus total et les informations alienvault nous permet de vou sassurer que cette ip est malveillante
- Qualification de 103.219.112.88:
>Criticité haute. cette ip doit être ajouté à toute vos listes noires.

### 4) 64.90.53.204 
	à la date du 9/11/2021 à 11h50
Cette ip à un score VirusTotal de 0/87, Elle apparaît aux états-unis d'amérique en californie (ASN:26347)
Elle est lié à l'Entreprise New Dream Network LLC. Son adresse IP CIDR est 64.90.53.204/24.
On peux trouver 74 noms de domaine et 21 Urls associés a cette IP.
Il semblerais que nous avons a faire à un Datacenter/Hébergeur/VPS
On trouve aussi six TopLevelDomain liés
3 ports sont ouvert sur cette machine. 
- Conclusion : La corrélation entre la classification en tant qu'un hébergeur et le nombre de noms de domaine et d'urls n'est pas inquiétant, il semble logique qu'un hébergeur possède de nombreux domaines.
- Qualification:
>Criticité  moyenne. Nous ne pouvons faire confiance à aucun artefacts provenant de 64.90.53.0/24 (apache2-sith.oakridge.dreamhost.com). Elle ne présente aucun rique a l'heure actuelle, mais un datacenter contient des systèmes de toute sortes pouvant présenter des menaces de différents niveaux.
>

### 5) 184.168.131.241 
	à la date du 9/11/2021 à 14H32
Cette ip à un score VirusTotal de 6/90 et une affluence de 20 commentaire alertent les utilisateur du rique que présente cette artefact. 
Elle apparaît aux etats-unis d'amérique en arizona (ASN:AS26496).
Elle est lié à l'entreprise GoDaddy.com, LLC. Son adresse IP CIDR est 184.168.131.0/24
Bloqué dans 15 DNs blocklists.
Alienvault :
* 2 port ouverts (80,443)
* 338 tags dont : tsec, tpot19, honeypot, ceber metre att, zeus, trojan etc...;
* 109 000 urls
* 63 000 fichiers
* détection antivirus 917/1000

- Conclusion : La correlation entre les alertes d'utilisateur virustotal et la quantité d'url et de fichiers liés nous montrent une forte aggressivité de la part de ce domaine.
les ports ouverts ne présentent pas de riques mais alienvault nous présentent de nombreux tags malveillant on suppose donc que certains sites web de GoDaddy.com sont truffés de malwares.
- Qualification:
>Criticité haute. De nombreux facteurs nous laissent penser que se connecter à un site de cette entité est un rique critique il faut absolument la bloquer.

### Conclusion
Nous préconisons une Mise en liste noire des IPs:
- 99.84.237.62
- 103.219.112.88
- 64.90.53.204 
- 184.168.131.241 
- 184.168.131.241 
il faut les ajouters en rêgles de pare-feu pour chacunes d'elles.
Du fait de la criticité de certaines IP, une analyse forensic de vos système à la recherche d'anomalies est conseillé.

Merci d'avoir fait appel à nos service nous restons à disposition pour de nouvelles demande d'analyse

Cordialement,
Corentin, "WideMorty" Lanoë , Responsable sécurité et des risques.


---
## Artefact streaming
Bonjour cher clients, clientes,
notre équipe d'analyses et de surveillance réseau vous rendent leur diagnostique au sujet des différentes Artefacts inhabituelles apparaîssant sur le réseaux de votre entreprise.
### 117.40.131.155
	démarré le 11/11/2021 à 18h00.
Cette ip à un score virustotal de 0/93, elle apparaît en Chine. (ASN: AS4134)

Elle possède en un proxy, un proxy en vpn et un vpn et est bloquée par certains DNSblocklist.
Elle est lié à l'entreprise China telecom; Son adresse CIDR est 117.40.131.0/24.

Cette ip à mauvaise réputation:
- IP réputation score 83
-alienvault; 6 urls ; tags malveillants: honeypot malicious IP, botnets mirai, blacklist, scan ; 6 port ouverts; 
présente des botnet en corrélation avec mirai.

- Conclusion : Un VPN est détecté donc on ne peux pas être sûr que le flux viennent sur le territoire chinois.
les tentative de déployer des botnet avec le tag mirai nous confirment que cette ip tente de faire de vos machine des zombies contrôlables à distance. Ell à déjà frappé car elle est blacklisté de certains entité (DNSblocklist)
- Qualitfication : 
>	Criticité haute. La source semble se cacher et s'attaquer a plusieurs entités, il est impératif de bloquer toute les communication avec elle.

### Conclusion
Nous préconisons un une mise en liste noire de l'ip et un sensibilisation de vos employés sur les site de flux vidéo utilisés.

Merci d'avoir fait appel à nos service nous restons à disposition pour de nouvelles demande d'analyse

Merci d'avoir fait appel à nos service nous restons à disposition pour de nouvelles demande d'analyse

Cordialement,
Corentin, "WideMorty" Lanoë , Responsable sécurité et des risques.


---

## Artefact Bittorrent
Bonjour cher clients, clientes,
notre équipe d'analyses et de surveillance réseau vous rendent leur diagnostique au sujet des différentes Artefacts inhabituelles apparaîssant sur le réseaux de votre département logiqstique. Nous commençons par détailler les riques de chaques adresses puis terminerons par des recommandations pour votre système.Bittorrent
### `http://download-lb.utorrent.com/endpoint/hydra-ut/os/win7/track/stable/cc-tag/290/browser/ie/os-region/US/os-lang/en/os-ver/6.1/enc-ver/111783726/`

	démarré le 11/11/2021 à 19h00
Cette url est détecté par Threatcrowd comme présentant de nombreux risques de malveillance (Opencandy).
Le relevé indique le fichier svhost.com, pour résumer il orchestre les modules ou service pour l'OS. Opencandy à donc pu se greffer à ce fichier, tourner en tâche de fond et consommer les ressources physique de l'ordinateur.
- Conclusion :OpenCandy est un adware, c'est à dire qu'il s'installe de pair avec un autre logiciel pour passer incognito. Votre ordianteur est probablement infecté.
Qualification:
>Criticité moyenne. Les ralentissement proviennet surment d'un adware qui s'est attaché au service svhost.com
Une analyse antivirus (premièrement heuristique puis antimalware, anti-rootkit, anti trojan qui ne sont pas la même chôse) ainsi que désinstaller tout les programmes inconnus sur le poste.

Nous ne pouvons pas vous conseillé d'outils ou de méthode malheureusement. La priorité est de trouver comment purger svhost.com et svhost.exe

### Conclusion
Dans le cadre professionnel un client bittorrent doit être utilisé prudemment et avec des sources de confiance.
Le system de votre employé est exposé à un rique d'infection.
Pour commencer nous préconisons de faire une analyse strict du système du poste client dans le but de purger le système puis réinstaller le programme windows: svhost.com & svhost.exe.

Dans un second temps ils nécessaire de sensibiliser vos employés à la vérification de la fiabilité des sources lors de téléchargement. 

Merci d'avoir fait appel à nos service nous restons à disposition pour de nouvelles demande d'analyse

Cordialement,
Corentin, "WideMorty" Lanoë , Responsable sécurité et des risques.


---








