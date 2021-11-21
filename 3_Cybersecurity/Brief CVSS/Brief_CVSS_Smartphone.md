# Catégorie deux : Smartphone
Les agents ZONE ont tous un iphone 12 pro de fonction et demande une note de vulnérabilité sur leur téléphone

---
## Bunker : Iphone 12 pro - OS Montery
*Un Bunker Israélien est le refuge d'un de nos agents qui rapporte avoir de nombreux PDF en double sur son disque dur*

###### CVE-2021-30919 : Vulnérabilité : PDF malveillant amenant à une écriture hors limites
>_An out-of-bounds write was addressed with improved input validation. This issue is fixed in iOS 15.1 and iPadOS 15.1, macOS Monterey 12.0.1, iOS 14.8.1 and iPadOS 14.8.1, tvOS 15.1, watchOS 8.1, Security Update 2021-007 Catalina, macOS Big Sur 11.6.1. Processing a maliciously crafted PDF may lead to arbitrary code execution._

[cvedetails](https://www.cvedetails.com/cve/CVE-2021-30919/)
[nvd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-30919)
**NVD Published Date:**  
08/24/2021  
**NVD Last Modified:**  
11/01/2021

* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-30919&vector=AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H&version=3.1&source=NIST)
 Nous donne un score CVSS de base de **7.8/10**
 Un fix a été appliqué pour cette vulnérabilité dans la [mise à jour](https://support.apple.com/en-us/HT212868) du 26 octobre 2021.

Le score passe de **7.8/10** à **7.5/10**

Qu'en est-il de notre score CVSS pour un poste dans un Bunker Israélien ?

Le contexte de notre vulnérabilité se place dans l'OS Montery sur Iphone 12 pro. à l'intérieur d'un bunker isolé du réseau WAN, seule une manipulation en Physique (MAV:P) est disponible, 
voyons comment la note CVSS évolue avec les paramètres environnementaux :
* **(AV) **L**ocal -> (MAV) **P**hysical

[Le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-30919&vector=AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H&version=3.1&source=NIST) devient un **6.3/10**

L'agent est isolé, tant qu'un zombie CPC ne lui décroche pas son téléphone des mains il est moins vulnérable.

---
## IT MegaCorp : Iphone 12 pro - OS Montery

*La ZONE possède un baie de farming et trading de cryptomonaies dans les locaux de Sony à Minato, Une soixantaine de PS4 tournent en continue pour les blockchains, Les Rigs sont supervisables  par un interface utilisateur sur mobile*

###### CVE-2021-30918 Problème sur l'écran de verrouillage (Lock Screen issue) 
>_A Lock Screen issue was addressed with improved state management. This issue is fixed in iOS 14.8.1 and iPadOS 14.8.1, iOS 15.0.1 and iPadOS 15.0.1. A user may be able to view restricted content from the Lock Screen._

[cvedetails](https://www.cvedetails.com/cve/CVE-2021-30918/)
[nvd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-30918)
**NVD Published Date:**  
08/24/2021  
**NVD Last Modified:**  
10/29/2021

* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-30918&vector=AV:P/AC:L/PR:N/UI:N/S:U/C:L/I:N/A:N&version=3.1&source=NIST)
Nous donne un score CVSS de **2.4/10**
Une mise à jour d'Apple du 1er octobre 2021 a résolu la vulnérabilité:
le score sur le temps modifie la note pour un score CVSS de **2.3/10**
[source IOS 14.8.1](https://support.apple.com/en-us/HT212868)
[source IOS 15.0.1](https://support.apple.com/en-us/HT212868)

Qu'en est-il du notre score CVSS pour un poste dans les locaux d'une multinationnale ?
* Il n'est pas extrème d'accéder au poste physiquement
* L'attaque se déploie assez facilement un fois devant un poste
* /!\ Il est intégré au réseau de l'entreprise, qui lui-même est lié au SI du groupe*
Exploitability Metrics
(AV) **L**ocal -> (MAV) **A**djacent **N**etwork

[Le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:P/AC:L/PR:N/UI:N/S:U/C:L/I:N/A:N/E:X/RL:O/RC:X/CR:X/IR:X/AR:X/MAV:A/MAC:X/MPR:X/MUI:X/MS:X/MC:X/MI:X/MA:X&version=3.1) du calculateur Nist avec les facteurs environnementaux :
Notre score monte, il atteint la note de **4.1/10**
L'entreprise étant ouvert sur l'extérieur augmente grandement la note, on peut néamoins espérer que les mises à jour de sécurité sont faites et que la vulnérabilité ne soit plus existante. 

---
## Salle Sécurisée : Iphone 12 pro - OS Montery

*Dans le Dubaï Mall, le monstre de l'urbanisme de luxe des Émirats arabes unis la salle sécurisé semble imprenable, mais il est possible que l'Iphone de notre agent Rogue ne le soit pas*

###### CVE 2021-## CVE-2021-30909
>_A memory corruption issue was addressed with improved memory handling. This issue is fixed in iOS 15.1 and iPadOS 15.1, macOS Monterey 12.0.1, iOS 14.8.1 and iPadOS 14.8.1, tvOS 15.1, watchOS 8.1, Security Update 2021-007 Catalina, macOS Big Sur 11.6.1. An application may be able to execute arbitrary code with kernel privileges._

[cvedetails](https://www.cvedetails.com/cve/CVE-2021-30909/)
[nvd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-30909)
**NVD Published Date:**  
08/24/2021  
**NVD Last Modified:**  
11/02/2021
* [Base score](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-30909&vector=AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H&version=3.1&source=NIST)
Nous donne un score CVSS de **7.8/10** en vu de la faible complexité de la mise en place de l'exploit, l'absence de privilèges requis et la criticité de l'impact de l'exploit.
Les mises à jour du 25 et 26 octobre résolvent les vulnérabilités.
sources:
Hyperlink

Resource:
[https://support.apple.com/en-us/HT212867](https://support.apple.com/en-us/HT212867)
[https://support.apple.com/en-us/HT212868](https://support.apple.com/en-us/HT212868)
[https://support.apple.com/en-us/HT212869](https://support.apple.com/en-us/HT212869)
[https://support.apple.com/en-us/HT212871](https://support.apple.com/en-us/HT212871)
[https://support.apple.com/en-us/HT212872](https://support.apple.com/en-us/HT212872)
[https://support.apple.com/en-us/HT212874](https://support.apple.com/en-us/HT212874)
[https://support.apple.com/en-us/HT212876](https://support.apple.com/en-us/HT212876)
Le score CVSS temporaire devient **7.5/10**.

Qu'en est-il du notre score CVSS pour un téléphone dans une salle sécurisé du plus grand centre commercial au monde avec une surface totale de 1 124 000 mètres carrés ?
- L'(AV) ne peut être que **L**ocal
- Les **CIA** ne peuvent pas être en **(H)**igh

[Le score de vulnérabilité](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?vector=AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H/E:X/RL:O/RC:X/CR:M/IR:M/AR:M/MAV:L/MAC:X/MPR:X/MUI:X/MS:X/MC:X/MI:X/MA:X&version=3.1) du calculateur Nist avec les facteurs environnementaux :

En prenant compte qu'un correctif existe depuis les versions 14.8.1 et 15.0.1 le score CVSS global devient **7.5/10**.

L'attaque n'est pas complexe à mettre en place et l'impact est high pour CIA
Le score CVSS reste sensiblement le même après le fix et la mise en place de l'environnement.

---