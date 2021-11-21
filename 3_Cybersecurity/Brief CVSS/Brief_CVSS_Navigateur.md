# Catégorie une : Navigateur
--- 
## Bunker : Microsoft edge
*La ligne Sokolnitcheskaïa du métro russe abrite un Bunker protégeant les plans de la navette spatiale Maya Labueï (майя лабей)*

###### CVE-2021-38669 : Vulnérabilité à la falsification(Tampering vulnerability)
>Microsoft Edge (Chromium-based) Tampering Vulnerability

[cvedetails](https://www.cvedetails.com/cve/CVE-2021-38669/)
[nvd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-38669)
**NVD Publish Date :** 
2021-09-15 
** NVDLast Update Date :**
2021-09-28
* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-38669&vector=AV:N/AC:L/PR:L/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST)
Nous donne un score CVSS de **8.8/10** (légèrement plus haut que sur cvedetails.com
Une mises à jour de Microsoft du 9 septembre 2021 a résolu la vulnérabilité :
le score sur le temps modifie la note pour un score CVSS de **7.7/10**
Le risque est moindre car une correction à été appliqué. 
[msrc.microsoft.com](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-38669)

Qu'en est-il de notre score CVSS pour un poste dans un Bunker russe ?

Le contexte de notre vulnérabilité se place dans le navigateur edge sur un poste informatique dans bunker isolé du réseau WAN, seule une attaque en local est possible voyons comment la note évolue avec les paramètres environnementaux :

* **(AV) **N**etwork -> (MAV) **P**hysical
* **(AC) **L**ow -> (MAC) **H**igh

[Le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:N/AC:L/PR:L/UI:N/S:U/C:H/I:H/A:H/CR:X/IR:X/AR:X/MAV:P/MAC:H/MPR:X/MUI:X/MS:X/MC:X/MI:X/MA:X&version=3.1) global devient **6.3/10**

Ces deux facteurs sont les raisons de la baisse du score, Premièrement le bunker est surveillé en continu donc cela rend l'accès physique à l'ordinateur extrêmement complexe.
Ensuite l'acces depuis l'éxtérieur est impossible, le Bunker ne possède pas d'accès au réseau externe ce qui rend la falsification compliquée dans notre cas.

---

## IT Mega Corp: Chromium/Microsoft Edge
*Les bureaux du Label Universal de Londres sont attaqués par l'entrée principale. Ils abritent de nombreux enregistrements secret défense de la ZONE. 
Acceuil : un rang de 3 postes allumés*

###### CVE-2021-21140 : Vulnérabilité USB (Out-Of-Bounds memory access via a USB device)
>_Uninitialized use in USB in Google Chrome prior to 88.0.4324.96 allowed a local attacker to potentially perform out of bounds memory access via a USB device._

[cvedetails](https://www.cvedetails.com/cve/CVE-2021-21140/)
[nvd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-21140)
**NVD Published Date:**  
02/09/2021  
**NVD Last Modified:**  
02/25/2021
  * [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-21140&vector=AV:P/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST) 
Nous donne un score CVSS de **6.8/10**
Une mise à jour de sécurité a résolu la vulnérabilité :
>_The vulnerability assigned to this CVE is in Chromium Open Source Software (OSS) which is consumed by Microsoft Edge (Chromium-based). It is being documented in the Security Update Guide to announce that the latest version of Microsoft Edge (Chromium-based) is no longer vulnerable. 
Source :Please see [Security Update Guide Supports CVEs Assigned by Industry Partners](https://msrc-blog.microsoft.com/2021/01/13/security-update-guide-supports-cves-assigned-by-industry-partners/) for more information._

Qu'en est-il de notre score CVSS pour un poste dans une tour de 50 étages ?
* Il n'est pas extrême d'accéder au poste physiquement
* L'attaque se déploie assez facilement une fois devant un poste
* /!\ Il est intégré au réseau de l'entreprise, qui lui-même est lié au SI du groupe.

Exploitability Metrics
(AV) **L**ocal -> (MAV) **A**djacent **N**etwork
Notre score CVSS monte, il atteint la note de **8.0/10**
L'entreprise étant ouvert sur l'extérieur augmente grandement la note, on peut néamoins espérer que les mises à jours de sécurité sont faites et que la vulnérabilité ne soit plus existante. 

---

## Salle sécurisée : Mozilla Firefox
*La Salle Sécurisé de l'entreprise OVH Télécom est accessible par un interstice du sous-sol que le CPC a creusé, la ZONE tremble.*

###### CVE-2020-15684 :Vulnérabilité sur la sécurité de la mémoire
>Mozilla developers reported memory safety bugs present in Firefox 81. Some of these bugs showed evidence of memory corruption and we presume that with enough effort some of these could have been exploited to run arbitrary code. This vulnerability affects Firefox < 82.

[cvedetails](https://www.cvedetails.com/cve/CVE-2020-15684/)
[vnd.nist](https://nvd.nist.gov/vuln/detail/CVE-2020-15684)
**NVD Published Date:**  
10/22/2020  
**NVD Last Modified:**  
07/21/2021
* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2020-15684&vector=AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST)
Nous donne un score CVSS de base de **9.8/10** en vue de la simplicité de la mise en place de l'exploit et de la criticité de l'impact de l'exploit.
 La vulnérabilité disparait après la mise à jour de sécurité de Mozilla Firefox 82.
[source](https://www.mozilla.org/en-US/security/advisories/mfsa2020-45/)

Qu'en est-il de notre score dans un environnement d'une salle sécurisé ?
- L'(AV) ne peut être que **L**ocal
- Les mesures d'impact ne peuvent pas être en **H**igh

[Résultat](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H/E:X/RL:O/RC:X/CR:X/IR:X/AR:X/MAV:L/MAC:L/MPR:N/MUI:N/MS:U/MC:L/MI:L/MA:L&version=3.1) du calculateur Nist avec les facteurs environnementaux:

En prenant en compte qu'un patch existe depuis la version 82 de Firefox notre CVSS global descend à **5.7/10**.

Les répercutions de l'exploitation de la vulnérabilité [CVE-2020-15684](https://nvd.nist.gov/vuln/detail/CVE-2020-15684) en local sur un navigateur Firefox dans une salle sécurisé est nettement moins critique.

---
