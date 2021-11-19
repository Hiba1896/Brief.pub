# Catégorie une : Navigateur
--- 
## Bunker : Microsoft edge
*La ligne Sokolnitcheskaïa du métro russe abrite un Bunker abritant les plan de la navette spatiale Maya Labueï (майя лабей)*
Vulnérabilité à la falsification(Tampering vulnerability)
[ncvedetails](https://www.cvedetails.com/cve/CVE-2021-38669/)
[nvd.nist](https://nvd.nist.gov/vuln/detail/CVE-2021-38669)
Publish Date : 2021-09-15 
Last Update Date : 2021-09-28
https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-38669&vector=AV:N/AC:L/PR:L/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST
nous donne un score de 8.8/10
(légèrement plus haut que sur [cvedetails.com](https://www.cvedetails.com/cve/CVE-2021-38669/))

Avec les mises à jours de microsoft  du le score sur le temps modife la note pour un score de 7.7/10
Le risque est moindre car une correction à été appliqué. 

Le contexte de notre vulnérabilité se place dans le navigateur edge sur un poste informatique dans bunker isolé du réseau WAN, seule une attaque en local est possible voyont comment la note évolue avec les paramètres environnementaux:
AV Network -> MAV Local
AC Low -> MAC High
Le score de vulnérabilité devient un 6.8/10

Ces deux facteurs sont les raisons de la baisse du score, Premièrement le bunker est surveillé en continu donc cela rend l'accès en local à l'ordinateur extrèmmement complexe.
Ensuite l'acces depuis l'éxtérieur est impossible, le Bunker ne possède pas d'accès au réseaux externe ce qui rend la falsification compliqué dans notre cas.

---

## IT Mega Corp: Chromium/Microsoft Edge
*Les bureaux du Label Universal sont attaqués par l'entrée principal, à l'acceuil un rang de 3 poste pour les agents d'acceuil*

vulnérabilité USB ( out of bounds memory access via via a USB device)
**NVD Published Date:**  
02/09/2021  
**NVD Last Modified:**  
02/25/2021
 **Base score**:
 https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2021-21140&vector=AV:P/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST 
nous donne un score de 6.8
Une mise à jour de sécurité aurais résolu la vulnérabilité :
>
The vulnerability assigned to this CVE is in Chromium Open Source Software (OSS) which is consumed by Microsoft Edge (Chromium-based). It is being documented in the Security Update Guide to announce that the latest version of Microsoft Edge (Chromium-based) is no longer vulnerable. 
Source :Please see [Security Update Guide Supports CVEs Assigned by Industry Partners](https://msrc-blog.microsoft.com/2021/01/13/security-update-guide-supports-cves-assigned-by-industry-partners/) for more information.

Quand est-il du notre score pour un poste dans une tour de 50 étages ?
* il n'est pas extrème d'accéder au poste physiquement
* l'attaque se déploie assez facilement un fois devant un poste
* /!\ il est intégré au réseau de l'entreprise, qui elle même est lié au SI du groupe*

Exploitability Metrics
**AV** Local -> **MAV** Adjacent Network
Notre score monte, il atteint la note de **8.0/10**
L'entreprise étant ouvert sur l'extérieur augmente grandement la note, on peux néamoins espérer que les mise à jours de sécurité sont faites et que la vulnérabilité soit réparé. 

---