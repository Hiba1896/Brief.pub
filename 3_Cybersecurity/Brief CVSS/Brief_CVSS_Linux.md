# Catégorie trois : Linux
La ZONE utilise des systèmes d'exploitation linux dans leurs infrastructures pour gérer leurs opérations sur Terre, les base de données sont en périls suite aux actions globales du CPC.

---
## Bunker : OpenSUSE
**

###### CVE-2017-5333 Débordement d'entier résultant un dénis de service ou l'éxecution de code arbitraire
>_Integer overflow in the extract_group_icon_cursor_resource function in b/wrestool/extract.c in icoutils before 0.31.1 allows local users to cause a denial of service (process crash) or execute arbitrary code via a crafted executable file._

[cvedetails](https://www.cvedetails.com/cve/CVE-2017-5333/)
[vnd.nist](https://nvd.nist.gov/vuln/detail/CVE-2017-5333)

* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2016-0051)
Nous donne un score CVSS de base de **7.8/10**
Un correctif a été appliqué pour cette vulnérabilité dans les mises à jour ( [1](https://lists.opensuse.org/opensuse-security-announce/2017-01/msg00026.html);[2](https://lists.opensuse.org/opensuse-security-announce/2017-01/msg00025.html); [3](https://lists.opensuse.org/opensuse-security-announce/2017-01/msg00024.html)) du 17 Janvier 2017.

Le score passe de **7.8/10** à **7.5/10**

Qu'en est-il de notre score CVSS pour un poste dans un Bunker ?

Le contexte de notre vulnérabilité se place dans l'OS Linux OpenSUSE à l'intérieur d'un bunker isolé du réseau WAN, seule une manipulation en Physique (MAV:P) est disponible, 
voyont comment la note CVSS évolue avec les paramètres environnementaux :
* **(AV) **L**ocal -> (MAV) **P**hysical

[Le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H/E:X/RL:O/RC:X/CR:X/IR:X/AR:X/MAV:P/MAC:X/MPR:X/MUI:X/MS:X/MC:X/MI:X/MA:X&version=3.1) CVSS devient un **6.3/10**


---

## IT MegaCorp : KALI 
*Les Zombies CPC reviennent du siège de Sony avec des milliers de clefs USB remplis d'outils plutôt intrusifs, Et se dirigents à pas de fourmies vers les Bureaux de Rogue Cervoise au siege *
####### CVE-2021-43976 Dénis de service avec un périphérique USB (Denial of service)
>_In the Linux kernel through 5.15.2, mwifiex_usb_recv in drivers/net/wireless/marvell/mwifiex/usb.c allows an attacker (who can connect a crafted USB device) to cause a denial of service (skb_over_panic)._

[cvedetails](https://www.cvedetails.com/cve/CVE-2021-43976/)
[vnd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-43976)

* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-43976&vector=AV:P/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H&version=3.1&source=NIST)
Nous donne un score CVSS de base de **4.6/10**
Un correctif a été appliqué pour cette vulnérabilité dans la [mise à jour](https://patchwork.kernel.org/project/linux-wireless/patch/YX4CqjfRcTa6bVL+@Zekuns-MBP-16.fios-router.home/) du 1er novembre 2021.

Le score passe de **4.6/10** à **4.4/10**

Qu'en est-il de notre score CVSS pour un poste dans les locaux d'une multinationnale ?
* Il n'est pas extrème d'accéder au poste physiquement
* L'attaque se déploie assez facilement une fois devant un poste
* /!\ Il est intégré au réseau de l'entreprise, qui-lui même est lié au SI du groupe*
Exploitability Metrics
(AV) **L**ocal -> (MAV) **A**djacent **N**etwork
Le contexte de notre vulnérabilité se place dans l'OS linux KALI dans les locaux d'une multinationale.
[Le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:P/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H/E:X/RL:O/RC:X/CR:X/IR:X/AR:X/MAV:A/MAC:X/MPR:X/MUI:X/MS:X/MC:X/MI:X/MA:X&version=3.1) CVSS devient un **6.2/10**

Le score monte, car on pourrait, selon le contexte, accéder à l'intégralité du service informatique après la réalisation de l'attaque.

---

## Salle Sécurisée : Arch linux
* _Battle music intensifies _ H-2 Du lancement de la navette, les Zombies CPC contre-attaquent sur la Salle sécuriséede la ZONE après leurs échecs chez les Rogues Cervoises*
###### CVE-2020-5291 BubbleWrap | Context Complexity (High) | (gain root permisison)
>_Bubblewrap (bwrap) before version 0.4.1, if installed in setuid mode and the kernel supports unprivileged user namespaces, then the `bwrap --userns2` option can be used to make the setuid process keep running as root while being traceable. This can in turn be used to gain root permissions. Note that this only affects the combination of bubblewrap in setuid mode (which is typically used when unprivileged user namespaces are not supported) and the support of unprivileged user namespaces. Known to be affected are: * Debian testing/unstable, if unprivileged user namespaces enabled (not default) * Debian buster-backports, if unprivileged user namespaces enabled (not default) * Arch if using `linux-hardened`, if unprivileged user namespaces enabled (not default) * Centos 7 flatpak COPR, if unprivileged user namespaces enabled (not default) This has been fixed in the 0.4.1 release, and all affected users should update._


Une seule vulnérabilité sur [cvedetails](https://www.cvedetails.com/cve/CVE-2020-5291/)
[vnd.nist](https://nvd.nist.gov/vuln/detail/CVE-2020-5291)

* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2020-5291&vector=AV:L/AC:L/PR:L/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST)
Nous donne un score CVSS de base de **7.8/10**
Un correctif a été appliqué pour cette vulnérabilité dans la [mise à jour V0.4.1 (git commit)](https://github.com/containers/bubblewrap/commit/1f7e2ad948c051054b683461885a0215f1806240) du 20 mars 2020.
Le score CVSS temporel devient **7.5/10**.


Qu'en est-il de notre score CVSS pour un poste dans une salle sécurisé ?

Le contexte de notre vulnérabilité se place dans l'OS linux
- L'(AV) ne peut être que **L**ocal
- Les mesures d'impacts ne peuvent pas être en **(H)**igh


VoyonS comment la note CVSS évolue avec les paramètres environnementaux :

* Metrics :Confidentiality (low) Integrity(Low) Availability(Low)
[Le score de vulnérabilité]()du calculateur Nist avec les facteurs environnementaux:
Notre score , il atteint le score CVSS **5.1/10**
* Metrics :Confidentiality (None) Integrity(None) Availability(None)
_Dans un contexte ou les métriques CIA serais insignifiants [le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:L/AC:L/PR:L/UI:N/S:U/C:H/I:H/A:H/E:X/RL:O/RC:X/CR:X/IR:X/AR:X/MAV:L/MAC:X/MPR:X/MUI:X/MS:X/MC:N/MI:N/MA:N&version=3.1)du calculateur Nist avec les facteurs environnementaux:
Notre score CVSS devient **0/10**_

Le vecteur d'attaque n'est pas modifée donc le score CVSS reste le même que le score temporel, les mesures d'impact sont baissé à **L**ow pour les impacts de confidentialité, d'intégrité et de disponibilité, ce qui fait chuter le score CVSS comparé au score de base, lorsque le contexte environnemental n'est pas définis.

---

Désolé pour la longueur et la répétitivité du rapport voici une patate douce, Merci pour votre lecture.
![miam|720x480](https://www.southernexposure.com/images/large/sweet-potato-ginseng_LRG.jpg)