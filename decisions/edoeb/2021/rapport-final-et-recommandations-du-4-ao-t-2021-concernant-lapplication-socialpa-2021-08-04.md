---
decision_id: "edoeb_rapport-final-et-recommandations-du-4-août-2021-concernant-lapplication-socialpa-2021-08-04"
court: "EDÖB"
court_id: "edoeb"
docket: "rapport-final-et-recommandations-du-4-août-2021-concernant-lapplication-socialpa-2021-08-04"
decided: "2021-05-31"
published: "2021-08-04"
language: "fr"
legal_area: "Datenschutz"
decision_type: "Schlussbericht/Empfehlung"
source_url: "https://www.edoeb.admin.ch/dam/de/sd-web/ZNJEjAp8ku7C/20210804_Rapport%20final%20et%20recommandations_SocialPass.pdf"
pdf_url: "https://www.edoeb.admin.ch/dam/de/sd-web/ZNJEjAp8ku7C/20210804_Rapport%20final%20et%20recommandations_SocialPass.pdf"
cites_law: ["switzerland/bund/acts/235.1/art-003.md", "switzerland/bund/acts/235.1/art-004.md", "switzerland/bund/acts/235.1/art-005.md", "switzerland/bund/acts/235.1/art-006.md", "switzerland/bund/acts/235.1/art-007.md", "switzerland/bund/acts/235.1/art-008.md", "switzerland/bund/acts/235.1/art-013.md", "switzerland/bund/acts/235.1/art-029.md", "switzerland/bund/acts/235.1/art-030.md", "switzerland/bund/acts/235.1/art-034.md", "switzerland/bund/acts/235.11/art-008.md", "switzerland/bund/acts/235.11/art-009.md", "switzerland/bund/acts/235.11/art-011.md", "switzerland/bund/acts/235.11/art-034.md", "switzerland/bund/acts/818.101/art-033.md"]
---

# Rapport final et recommandations du 4 août 2021 concernant l'application "SocialPass"PDF4.65 MB4. August 2021

## Text

Schweizerische Eidgenossenschaft
Confederation suisse
Confederazione Svizzera
Confederaziun svizra
Prepose federal ä la protection des donnees et ä la transparence
PFPDT
Rapport final et recommandations
du Prepose federal a la protection des donnees et a la transparence
(PFPDT)
du 4 aoüt 2021
dans le cadre
de la procedure d'etablissement des faits selon l'article 29
de la Loi federale sur la protection des donnees du 19 juin 1992
(LPD ; RS 235.1)
concernant
l'application « SocialPass »
de SwissHelios Sari, a Oberlunkhofen
et NewCom4U Sari, a Sierre
representees par Lexing Switzerland, 1951 Sion
Uusqu'au 14 juin 2021)
Feldeggweg 1, 3003 Berne
Tel. 058 463 74 84, Fax 058 465 99 96
www.edoeb.admin.ch

0
Table des matiëres
1. Introduction........................
1.1 .
Remarques prëliminaires ......
1.2.
Situation de dëpart...
1.3. Parties impliquëes ...............
1.4. Chronologie
des ëvënements
. .............................
1.5.
Portëe de la procëdure d’ëtablissement des faits.
1.6.
Bases de l’ëtablissement des faits..
1.7.
Analyses effectuëes dans le cadre de la prësente procëdure.
1.8.
Bases lëgales.
1.9.
Compëtence du PFPDT..
2.
Faits ëtablis
2.1 .
Röles et responsabilitës....... .
2.2.
Composants et fonctions ..... ,
2.2.1 .
ApeQU ..........................
2.2.2.
Description du processus d'enregistrement ....,
2.2.3.
Fonctions de SocialScan .....,... .
2.2.4.
SocialPass : enregistrement et utiËisation
2.2.5.
Base de donnëes centralisëe .
a.
Gënëralitës............................,
b.
Accës des autoritës cantonales aux coordonnëes des clients .. ,
2.3.
But de la collecte des donnëes..........
2.4.
Description des diffërents modes de fonctionnement.
2.4.1.
SocialScan : saisie manuelle (enregistrement des clients rëguliers) .
2.4.2.
Stockage des numëros de tëlëphone mobile issus du processus d’e
2.5.
Services de tiers ...............................
2.5.1 .
Infomaniak ..
2.5.2.
Twilio .......................................,
2.5.3.
Microsoft Azure (base de donnëes SQL) ....
2.6.
Information et droits des personnes concernëes..,
2.6.1 .
Information des utilisateurs . ................
,
2.6.2.
Droits des personnes concernëes ......
a.
Exercice du droit d’accës .
b.
Exercice du droit ä l’effacement des donnëes.....................................,
2.7.
Aspects de sëcuritë des donnëes..
.. 7
10
11
12
13
13
13
13
14
14
15
17
17
19
19
20
23
24
24
26
26
26
26
27
27
27
28
28
28
28
lregistrement .
2/62

0
2.7.1.
Organisation de la sëcuritë de 1’information
Login avec double-authentification
Identifiants de I'utilisateur ...........,
28
29
29
29
29
31
32
32
32
32
33
33
34
34
36
36
36
36
36
37
37
37
37
37
37
37
38
38
38
38
38
38
38
39
39
2.7.2.
2.7.3.
2.7.4.
Gëolocalisation ...........................,
2.8
Analyse de 1’audit de Navixia SA ,
2.8.1.
Interaction avec la plateforme (6.2.6 et 6.3.6)
2.8.2.
Qualitë du code et packaging (6.3.7)
2.8.3.
Descripteur
(7.1) ...............................,
2.8.4.
Mots de passe stockës en clair (7.1 )
2.8.5.
Conservation des donnëes (8.4.1).
2.9. Analyse de I'audit d’lndusface ....................
2.9.1 .
Classification .......,
2.9.2.
Rësultats en fonction des catëgories ..
2.9.3.
Android et iOS Mobile .
2.9.4.
Conclusions de I'audit Indusface ..,
a.
Blind HTML Injection [1]..,
Insecure Direct Object References [2] ...,
Insecure Logging Of The Application [4]
Application is Vulnerable To Improper Token Management [5] .. .
Application Accepts Special Character As User Input [6] .
Valid Account Can Be Brute Forced [7] ...............................
b.
c.
d.
e.
f.
Missing API Rate Limiting [8] ........,
Application Does Not Have A Strong Password Policy [9]
Cleartexttraffic is Set To True [1 1 ]
Application is Vulnerable To Simultaneous Login [12] ................
Application's Request/Response Reveals Sensitive Information
SSL Pinning Can Be Bypassed [14] ...........................................,
Insecure Data Storage in File System [15] . ,
Insecure Content Security Policy (Csp)/X-Frame-Options [16] ...
Missing HSTS Header [17] .,
Information Leakage From Clipboard [18] ..,
q.
Sensitive Data Disclosure in Recent Apps [19] ....
r.
Application Has Set Insecure Permissions [21 ]
Apprëciation juridique et recommandations ...
Röles et responsabiIËtës... ,
g.
h.
i.
j.
k.
[13]
1.
m
n.
0.
P.
3,
3.1
3/62

0
Banque de donnëes centralisëe ....................
Banque de donnëes centralisëe stricto sensu .........
Divers droits d'accës ä la base de donnëe centralisëe / fonctions de filtres
Option « saisie manuelle » ..................,..............
Transferts des numëros de tëlëphone aux Ëtats-Unis ... .
Stockage centralisë et permanent du numëro de tëlëphone mobile dans le processus
d'enngistnment
....................................................................................................................
49
3.6.
Microsoft Mun (base de donnëes SQL) ..............................................................................
50
3.7.
Divers aspects de sëcuritë des donnëes...............................................................................
50
3.7.1.
Gestion
des vulnërabilitës..............................................................................................
51
3.7.2.
Mise en place d’une authentification
forte .................................................,...................
51
3.7.3.
Utilisation disproportionnëe d'identifËants ......................................................................
51
3.7.4.
Organisation et documentation relatives ä la sëcuritë des donnëes . ............................
52
Prises de position des parties ........................................................................................................
53
4.1.
Remarques prëliminaires relatives au droit d’ëtre entendu ...................................................
53
4.2.
Prise de position des parties relative aux faits ëtablis Ie 20 mai 2021 ..................................
53
4.3.
Prise de position des parties relative au rapport final et aux recommandations du 28 mai
2021 .......................................................................................................................................
54
4.3.1.
Recommandation (1) concernant les röles et les responsabilitës .................................
54
4.3.2.
Recommandation (2) concernant Ia base de donnëes centrale....................................
55
4.3.3.
Recommandation (3) concernant Ia liste des clients rëguliers SocialScan .................. . 55
4.3.4.
Recommandation (4) concernant Ie service de vërËfication des numëros....................
. 56
4.3.5.
Recommandation (5) concernant l’enregistrement centralisë et permanent du numëro
de tëlëphone mobile dans le processus d'enregistrement ............................................
57
Recommandation (6) concernant la configuration et le renforcement de Microsoft Azure
58
Recommandation (7) concernant la gestion des vulnërabilitës.....................................
58
RecommandatËon (8) concernant la mise en place d'une authentification forte ............ 59
Recommandation (9) concernant le traitement des identifiants d'appareils..................
59
Recommandation (10) concernant la documentation relative ä la sëcuritë des donnëes
3.2.
3.2.1 .
3.2.2.
3.3.
3.4.
3.5.
41
41
43
47
48
4.
4.3.6.
4.3.7
4.3.8.
4.3.9,
4.3.10,
5.
Conclusion
6. Suite de la procëdure ...................
7.
Publication de la recommandation en vertu de I'art. 30 al. 2 LPD
,.... 60
,..... 61
..61
4/62

0
1. Introduction
1.1.
Remarques prëliminaires
Le Prëposë fëdëral ä la protection des donnëes et ä la transparence (PFPDT) ëtablit les faits d’office ou
ä la demande de tiers lorsqu'une mëthode de traitement est susceptible de porter atteinte ä la
personnalitë d'un nombre important de personnes (erreur de systëme ; art. 29 LPD).
La prësente procëdure a pour but de permettre au PFPDT de vërifier si les principes de la protection
des donnëes tels que fixës aux articles 4 et 7 LPD et les prescriptions sanitaires en matiëre de tra9age
sont respectës dans le cadre de l’exploitation et l’utilisation du systëme SocialPass.
1.2.
Situation de dëpart
Dans Ie but de mieux lutter contre la pandëmie de COVID-19, le Conseil fëdëral a prëvu dans
l’Ordonnance sur les mesures destinëes ä lutter contre l’ëpidëmie de COVID-19 en situation particuliëre
du 22 juin 2020 (Ordonnance Covid-19 situation particuliëre ; RS 818.101.26) que les exploitants
d’installations ou d'ëtablissements accessibles au public doivent cotlecter les coordonnëes des
participants ou des visiteurs. La collecte des coordonnëes (donnëes personnelles au sens de 1’art. 3
lit. a LPD) a pour but de pouvoir retracer des cas d’ëventuelles infections au sein d’un restaurant ou de
tout autre ëtablissement ou ëvënement accessible au public. Ä cette fin, les exploitants et les
organisateurs sont tenus de collecter le nom, le prënom, le domicile et le numëro de tëlëphone de leurs
clients (ch. 4.4. lit. a de l’Annexe 1 Ordonnance COVID-19 situation partËculiëre). L’art. 5 Ordonnance
COVID-19 situation particuliëre prëcise que les personnes concernëes doivent ëtre informëes de cette
coIËecte de donnëes et du but de l’utilisation de leurs donnëes (tragage des contacts). Les coordonnëes
doivent ëtre immëdiatement transmises par voie ëlectronique au service cantonal compëtent s’iI en fait
la demande aux fins d’identification et d’information des personnes prësumëes infectëes au sens de
1’art. 33 de la Loi sur les ëpidëmies (LEp ; RS 818.101). De surcroit, l’Ordonnance situation particuliëre
fixe que les coordonnëes collectëes ne peuvent pas ëtre utilisëes ä d'autres fins que celle du tra9age et
qu'elles doivent ëtre conservëes durant les 14 jours suivant Ia visite de l’ëtablissement puis
immëdiatement dëtruites.
Afin de faciliter la collecte desdites donnëes dans le cadre de la lutte contre la pandëmie, les sociëtës
SwissHelios et NewCom4U ont dëveloppë SocialPass. Ce systëme est composë essentiellement de
trois composants : 1’application SocialPass peut ëtre tëlëchargëe sur l’appareil mobile des clients et
visiteurs tandis que 1’application SocialScan est utilisëe par les ëtablissements accessibles au public
comme p.ex. les restaurants. Les donnëes sont ensuite stockëes sur une base de donnëes centrale
Dans le cadre de la prësente procëdure le terme < SocialPass » fera rëfërence - sauf mention contraire
– au systëme entier, englobant notamment les applications mobiles SocialPass et SocialScan ainsi que
la base de donnëes centralisëe.
5/62

0
Ä partir du mois dejuillet 2020, le PFPDT a regu plusieurs demandes de citoyens ainsi que des mëdias
suggërant que les traitements de donnëes tels que prëvus par SocialPass violeraient potentiellement le
cadre lëgal prëvu par la LPD et les prescriptions sanitaires en matiëre de tra9age. Dans le cadre de sa
fonction d’autoritë de surveillance, le PFPDT a alors pris contact avec les responsables de ladite
application en novembre 2020. Cette prise de contact devait permettre au PFPDT de vërifier si les
critiques ëmanant de la sociëtë civile d'une part et de la presse d’autre part ëtaient fondëes. Dans Ie but
d'apporter des rëponses plus prëcises aux questions soulevëes lors de la premiëre prise de contact en
automne 2020, le PFPDT a ouvert, en dëcembre 2020, une procëdure d'ëtablissement des faits selon
1’art. 29 LPD, d’abord ä l’encontre de la SwissHelios Särl, puis ä l’encontre de la NewCom4U Särl. Les
deux procëdures ont ëtë formellementjointes Ie 4 mars 2021.
1.3.
Parties impliquëes
Les personnes physiques et morales ayant un röle dëterminant dans la prësente procëdure
d’ëtablissement des faits sont les suivantes
Exploitants de SocialPass:
SwissHelios Särl, Wiesenstrasse 7a, 8917 Oberlunkhofen, agissant par M. Erwin Peter, associë et
prësident des gërants et M. Julio Salgado, associë et gërant ;
NewCom4U Särl, Technopöle 3, 3960 Sierre, agissant par M. Thierry Pilet, associë et gërant ;
reprësentëes par Me Sëbastien Fanti, Me Gëraldine Gianadda et Me Alexandre Staeger. avocats au
sein de I'ëtude Lexing Switzerland Särl, Rue de Prë-Fleuri 8B, 1951 Sion
Responsables du dossier auprës du PFPDT :
Nathalie Weber, Cheffe Team 1, Domaine de direction protection des donnëes
Myriam Christ, Juriste Team 1, Domaine de direction protection des donnëes
Fritz von Allmen, Spëcialiste en sëcuritë informatique, Centre de compëtence IT et Sociëtë numërique
Michael Burger, Spëcialiste en sëcuritë informatique, Centre de compëtence IT et Sociëtë numërique
6/62

0
1.4.
Chronologie des ëvënements
Juillet-Oct. 2020
Plusieurs indices de la part de la sociëtë civile, des mëdias et de la Fëdëration
romande des consommateurs par rapport ä des traitements de donnëes effectuës
par I'application SocialPass potentiellement contraires au cadre lëgal.
Prise de contact par le PFPDT par ëcrit aprës un ëchange tëlëphonique avec
SwissHelios Särl Ie 23.10.2020, demande de prëcisions quant ä la confidentialltë
et la sëcuritë des donnëes et la double authentification.
Courriel du PFPDT ä SwissHelios Särl concernant la demande du 23.10.2020
restëe sans rëponse, questions complëmentaires avec dëlai de rëponse jusqu'au
09.11.2020.
Demande de SwissHelios Särl de mettre le cabinet d'avocats Lexing Switzerland,
Sion en copie.
Courriel de Lexing Switzerland informant le PFPDT d’intervenir pour SwissHelios
Särl, demande d’adresser toute correspondance ultërieure ä Lexing Switzerland
(ëlection de domicile en l’ëtude Lexing Switzerland).
Courriel de SwissHelios Särl au PFPDT, complëment aux rëponses re9ues par
Lexing Switzerland, NewCom4U Särl fait sa premiëre apparition dans la prësente
affaire et lit ce courriel en copie.
Courriel du PFPDT ä SwissHelios Särl, accusë de rëception des rëponses
sommaires, reprise de contact prëvue aprës ëvaluation interne des rëponses
regues.
Courriel de SwissHelios
Särl d'adresser
toute communication
ultërieure
directement ä SwissHelios Särl
Courriel du PFPDT ä Lexing Switzerland de la demande de SwissHelios Särl de
communiquer directement avec SwissHelios.
(_,ourriel du PFPDT ä SwissHelios Särl et NewCom4U Särl demandant des
prëcisions jusqu’au 04.12.2020.
Courriel du PFPDT ä SwissHelios Särl et NewCom4U Särl, rappel suite ä la
demande du 26.11.2020 restëe sans rëponse, rëponse par NewCom4U Särl
faisant valoir des problëmes linguistiques.
Courriel du PFPDT ä SwissHelios Särl et NewCom4U Särl concernant les
problëmes linguistiques mis en avant par les exploitants.
Courrier recommandë
(avec copie prëalable par courriel) du PFPDT ä
SwissHelios Särl (Ie 18.12.2020) et ä NewCom4U Särl (Ie 23.12.2020), demande
23.10.2020
03.11.2020
03.11.2020
09.11.2020
09.11.2020
10.11.2020
10.11.2020
11.11.2020
26.1 1.2020
07.12.2020
08.12.2020
18./23.12.2020
7/62

0
de prëcisions du 26.11.2020 restëe sans rëponse, ouverture de la procëdure
d’ëtablissement des faits selon l’art. 29 LPD
Courriel de Lexing Switzerland au PFPDT demandant une prolongation du dëlai
de rëponse, prolongation accordëe par le PFPDT par courriel du 12.01.2021.
Courriel de Lexing Switzerland au PFPDT, envoi de trois documents (Privacy and
Cookies Policy – socialpass – 14102020.docx ; Rapport technique SocialPass
14.01 .2021. pdf ; Rëponses aux questions – PFPDT.docx)
Courriel de Lexing Switzerland au PFPDT, envoi d'une procuration (incomplëte[
Courriel de Lexing Switzerland au PFPDT, envoi d’une procuration (complëte)
pour le compte de NewCom4U Särl.
Ëchange
tëlëphonique entre SwissHelios'
Särl et le PFPDT
concernant
la
reprësentation de SwissHelios Särl par Lexing Switzerland.
Courriel du PFPDT ä Lexing Switzertand, accusë de rëception des documents
re9us, dëlai pour soumettre les documents manquants fixë au 10.02.2021.
Courriers du PFPDT ä Lexing Switzerfand et ä SwissHelios Särl, avis relatif ä la
jonction prëvue des procëdures, soumission de questions supplëmentaires
(responsables des traitements de donnëes, dëtails sur le transfert des numëros
de tëlëphone aux Etats-Unis), dëlai de rëponse fixë au 17.02.2021.
Courriel de Lexing Switzerland au PFPDT, soumission de deux rapports d’audit.
Courrier de Lexing Switzerland au PFPDT, demande de prolongation de dëlai
Courrier du PFPDT ä Lexing Switzerland, prolongation de dëlai accordëe, au
26.02.2021 pour la question de la jonction de procëdure, au 05.03.2021 pour les
rëponses aux questions supplëmentaires.
Courriers du PFPDT ä Lexing Switzerland et ä SwissHelios Särl, avis relatif ä la
jonction dëfinitive des procëdures, demande de prëcisions, demande de divers
documents manquants, questions supplëmentaires sur divers aspects restës peu
clairs, dëlai fixë au 17.03.2021 (entrant).
Courrier de Lexing Switzerland au PFPDT, avec des rëponses sur la question du
maTtre du fichier (SwissHelios Särl) et concernant le transfert des numëros aux
Etats-Unis.
Courrier de Lexing Switzerland au PFPDT, confirmant d’intervenir au nom et pour
Ie compte de NewCom4U Särl et de SwissHelios Särl (une procuration serait
fournie ultërieurement), comprenant un nombre d’annexes et de rëponses aux
questions posëes.
Courriel de NewCom4U Särl au PFPDT, envoi du rapport Navixia.
11.01.2021
14.01.2021
15.01.2021
26.01.2021
29.01.2021
03.02.2021
09.02.2021
11.02.2021
18.02.2021
19.02.2021
04.03.2021
05.03.2021
17.03.2021
19.03.2021
8/62

0
22.03.2021
Courriel de Lexing Switzerland au PFPDT prëcisant que SwissHelios Särl estime
qu’une procuration formelle n’est pas nëcessaire, confirmation qu’aucun autre
document ëtait disponible.
Courriel de NewCom4U Särl au PFPDT soumettant quelques informations
actualisëes sur SocialPass.
Courrier du PFPDT ä Lexing Switzerland, recommandation provisoire d'adapter
au plus vite les possibilitës de traitements de maniëre ä ce qu'il soit possible
d’exploiter l’application en conformitë avec le droit fëdëral (avant la rëouverture
des restaurants).
Courriel du PFPDT
ä
Lexing Switzerland,
le courrier du
07.04.2021
(recommandations provisoires) ëtant restë sans retour demande de confirmer
jusqu’au 26.04.2021 que les fonctions de recherches cibËëes seront adaptëes
ainsi que comment et dans quel dëlai cela serait fait.
Courrier de Lexing Switzerland informant le PFPDT que la recommandation
provisoire ne sera pas suivie, soumission de divers documents.
Courrier du PFPDT ä Lexing Switzerland, notification des faits ëtablis
provisoirement et possibilitë de prësenter des remarques aux faits ëtablisjusqu’au
27.05.2021 (entrant) mentionnant qu’au vu de la rëouverture probable de
l’intërieur des restaurants Ie 31.05.2021, une prolongation de dëlai ëtait exclue.
Courrier de Lexing Switzerland au PFPDT, demande de prolongation de dëlai de
rëponse d’au moins 30 jours.
Courrier du PFPDT ä Lexing Switzerland, refus de la demande de prolongation
de dëlai notant que des remarques pourront toujours ëtre faites dans le dëtai
imparti.
Courrier de Lexing Switzerland
au PFPDT, demande de rëcusation des
collaborateurs en charge du dossier.
Courrier du PFPDT ä Lexing Switzerland, dëcision de non-entrëe en matiëre par
rapport ä la demande de rëcusation (et notification de la dëcision aux
Commissions de gestion des Chambres fëdërales en tant qu’autoritë de
surveillance du PFPDT).
Courrier du PFPDT ä Lexing Switzerland, clöture et notification du rapport final
et des recommandations, les parties disposent d'un dëlai de 30 jours pour
prendre position
Courriel de GastroVaud, GastroValais et les exploitants de SocialPass adressë
au PFPDT, aux Prëposës cantonaux vaudois et valaisans et aux Mëdecins
cantonaux vaudois et valaisans, proposition d’une visËoconfërence.
25.03.2021
07.04.2021
21.04.2021
23.04.2021
20.05.2021
21.05.2021
25.05.2021
27.05.2021
28.05.2021
28.05.2021
01.06.2021
9/62

0
07.06.2021
1ë’' visioconfërence organisëe par GastroVaud ä laquelle participent, entre autres,
les exploitants de SocialPass et teur avocat (agissant ëgalement en tant que
Prëposë valaisan ä la protection des donnëes), une reprësentante de la Prëposëe
ä la protection des donnëes du canton de Vaud, les mëdecins cantonaux vaudois
et valaisans et le Prëposë fëdëral, M. Adrian Lobsiger, aËnsi que trois
reprësentants de son autoritë. Proposition d’une dëmonstration du systëme par
les exploitants de SocialPass dans le cadre d’une deuxiëme visioconfërence.
Courrier du PFPDT ä Lexing Switzerland
rësumant
les rësultats de la
visioconfërence du 07.06.2021.
Courrier de Lexing Switzerland au PFPDT notifiant Ia fin du mandat de Lexing
Switzerland dans la prësente procëdure.
Courriel de SwissHelios Särl au PFPDT par rapport ä une dëmonstration du
systëme, demande de prolongation de dëlai de 30 jours pour commenter le
rapport final, la demande de rëcusation du 27.05.2021 est retirëe.
2ë’"' visioconfërence organisëe par les exploitants de SocialPass ä laquelle ont
participë, entre autres, les collaborateurs du PFPDT en charge du dossier, les
mëdecins cantonaux vaudois et valaisans, la prëposëe cantonaFe vaudoise et le
reprësentant lëgal de GastroVaud.
Courrier du PFPDT ä SwissHelios Särl et NewCom4U Särl, confirmation de la
prolongation de dëlai jusqu'au 16.07.2021.
Soumission de la prise de position des exploitants de SocialPass.
Clöture de la procëdure d’ëtablissement des faits et notification du rapport
final complëtë, avis de la publication du prësent rapport sur Ie site internet du
PFPDT
08.06.2021
14.06.2021
18.06.2021
24.06.2021
29.06.2021
09.07.2021
04.08.2021
1.5.
Portëe de la procëdure d’ëtablissement des faits
La prësente procëdure a pour but de permettre au PFPDT de vërifier si les principes de la protection
des donnëes tels que fixës notamment aux articles 4 et 7 LPD ainsi que les prescriptions sanitaires en
matiëre de tra9age sont respectëes dans le cadre de la gestion de SocialPass.
Les analyses portent essentiellement sur la question de savoir quels traitements de donnëes sont
effectuës par SocialPass. II convient de distinguer ces traitements du traitement (ëventuellement plus
ëtendu) de donnëes effectuë par les ëtablissements accessibles au public et de l’ëventuel traitement
ultërieur par les autoritës cantonales compëtentes (en cas d’infection au COVID-19).
La prësente
procëdure porte essentiellement sur
le traitement des donnëes
des visiteurs
d’ëtablissements ou d’ëvënements ; Ë'application SocialScan, utilisëe par les ëtablissements, n'est
10/62

0
incluse dans la prësente procëdure que dans la mesure oü elle est pertinente au regard des donnëes
des visiteurs.
Dans cette perspective, le PFPDT examine les aspects suivants du traitement des donnëes dans le
cadre de I'utilisation de I'application SociatPass :
Quels sont les types de traitements de donnëes effectuës par SocialPass ?
Quelles sont les catëgories de donnëes personnelles traitëes dans le cadre de l’utilisation de
SocialPass ?
Qui traite les donnëes ?
Dans quel but les donnëes sont-elles traitëes, pour quelle durëe ?
Quelles mesures de sëcuritë et de protection des donnëes ont ëtë mises en place ?
Les traitements
de donnëes effectuës lors de la visite du site web www.socialpass.ch
ne font
expressëment pas l’objet de la prësente procëdure. De mëme, les traitements de donnëes effectuës
lors du tëlëchargement de 1’application SocialPass ou SocialScan dans I'AppStore ou dans le PlayStore
ne sont pas analysës dans le cadre de la prësente procëdure. Les composants du systëme et
les sites web des deux entreprises SwissHelios et NewCom4U n'ont pas non plus ëtë examinës en
profondeur. II est apparu, lors de I'examen initial, que ces composants ne sont pas directement
impliquës dans le traitement des donnëes des personnes concernëes, respectivement qu'il n’existe pas
d'interfaces ou de flux de donnëes vers les coordonnëes collectëes.
1.6.
Bases de l’ëtablissement des faits
Le PFPDT s'appuie sur les sources suivantes pour la prësente procëdure d’ëtablissement des faits:
Informations accessibles au public, notamment sur Ie site web www.socialpass.ch et dans
I'AppStore (iOS) et le PlayStore (Android) ;
Correspondance avec les reprësentants de SwissHelios et NewCom4U depuis l’automne
2020 ;
Rapports d’audits et documents supplëmentaires fournis par les parties selon Ie tableau ci-
dessous.
Audits
Tableau 1: Rapports d’audit
RaI>port d’audit
Auteur
Date
[A]
[B]
GVD7009 Recheck SocialPass_SocialScanv1.2.pdf
iOS Mobile Application Audit Report of Social Scan
v1 .0.pdf
Navixia
Indusface
18.03.2021
04.1 1 .2020
11/62

0
[c]
Android Mobile Application Audit Report of Social
Scan v1.0.pdf
Indusface
04.11.2020
Documents supplëmentaires
Tableau 2: Documents rëfërencës complëmentaires
Document
Date
Auteur
[D]
[E]
[F]
[G]
[H]
[1]
[J]
[K]
Rapport technique SocialPass 14.01.2021.pdf
Fanti Diagramme.pptx
SocialPass - SocialScan Uebersicht - d.pdf
Rëponses aux questions PFPDT 17032021 - scan.pdf
2021 03 11 QuestionnaireTechniqueVI.pdf
Azu re-Sentinel-whitepaper. pdf
Privacy and Cookies Policy - socialpass -
14102020.docx
2021 03 11 QuestionnaireTechnique.docx
L. Miceli
S. Fanti
SocialPass
A. Staeger
L. MËceli
Microsoft
SwissHelios
14.01.2021
09.1 1.2020
09.1 1.2020
17.11.2021
17.03.2021
17.03.2021
10.10.2020
PFPDT
1 1 .03.2021
Ä plusieurs reprises le PFPDT s’est adressë aux exploitants de 1’application pour savoir si d'autres
informations et documents pertinents ëtaient disponibles pour assurer le meilleur dëroulement possible
de la prësente procëdure. Le PFPDT souhaitait notamment savoir quels composants du systëme
avaient fait l’objet de contröles de sëcuritë, le cas ëchëant par des spëcialistes externes, et s'il existait
des rësultats documentës, par exemple sous la forme d'ëvaluations de sëcuritë et de rapports de
vulnërabilitë
En dehors des documents mentionnës dans ce sous-chapitre, les exploitants de 1’application ont assurë
Ie PFPDT qu'aucun examen de ce type (par exemple pour le stockage de donnëes chez Microsoft
Azure) n'a ëtë effectuë et qu'ils ëtaient donc dans l’impossibilitë de transmettre les rësultats d'un tel
examen au PFPDT.
1.7.
Analyses effectuëes dans le cadre de la prësente procëdure
L’analyse technique de I'application SocialPass du PFPDT s’appuie sur les rapports d’audit des
entreprises Indusface du 4 novembre 2020 et Navixia du 18 mars 2021 ainsi que sur les documents
supplëmentaires soumis au PFPDT par les reprësentants des sociëtës SwissHelios et NewCom4U.
Lesdits rapports d’audit ont ëtë rëdigës entre les moËs d'octobre 2020 et mars 2021,
Aucune inspection des lieux en compagnie des responsables de SocialPass n’a eu Ëieu. Ainsi, toutes
les informations - tant de nature technique que juridique – qui ont ëtë jugëes dëterminantes pour
l’ëtablissement des faits ont ëtë exigëes des reprësentants lëgaux des sociëtës SwissHelios et
NewCom4U par ëcrit. Les questions du PFPDT s’appuyaient sur le cadre lëgal tel que prëvu par la LPD
12/62

0
et les prescriptions sanitaires en matiëre de tragage, la norme ISO 27002 ainsi que sur 1’Open Web
Application Security Project (OWASP)
1.8.
Bases lëgales
Les bases lëgales suivantes sont pertinentes dans le cadre de la prësente procëdure :
Loi fëdërale du 19juin 1992 sur la protection des donnëes (LPD), RS 235.1
-
Ordonnance du 14juin 1993 relative ä la lot fëdërale sur la protection des donnëes (OLPD),
RS 235.11
Loi fëdërale sur la lutte contre les maladies transmissibles de I'homme (Loi sur les ëpidëmies,
LEp), RS 818.101
Ordonnance sur les mesures destinëes ä lutter contre l’ëpidëmie de COVID-19 en situation
particuliëre du 19 juin 2020 (Ordonnance COVI D-19 situation particuliëre), RS 818.101.26
1.9.
Compëtence du PFPDT
En vertu de 1’art. 2 al. ler LPD, la LPD rëgit le traitement de donnëes concernant des personnes
physiques et morales effectuë par des personnes privëes (physiques ou morales). La prësente
procëdure d’ëtablissement des faits se penche sur diffërents traitements de donnëes effectuës par des
entitës privëes, notamment la collecte puis l’enregistrement des coordonnëes des visiteurs effectuës
par les exploitants d'ëtablissements ouverts au public dans le cadre de la lutte contre la pandëmie du
(_,OVID-19. Dës lors, la collecte des coordonnëes des visiteurs teIle que prëvue par l’Ordonnance
COVID-19 situation particuËiëre est une activitë privëe soumise ä la LPD et par consëquent ä la
surveillance du PFPDT. Au contraire, le traitement des donnëes (ultërieur) par les autoritës cantonales
(mëdecin cantonal, direction de la santë publique, ëquipe de tragage) tombe sous la surveillance des
prëposës cantonaux respectifs
2. Faits ëtablis
2.1.
Röles et responsabilitës
Fort,e est de constater qu’au bas du site web www.socialpass.ch consacrë ä 1’information des
citoyennes et citoyens, les coordonnëes de Swisshelios Särl ainsi que celles de HotelPro4U (produit de
marketing dëveloppë par la sociëtë NewCom4U Särl) sont mentionnëes. Ainsi, sur Ie site web, les deux
sociëtës apparaissent comme co-ëditrice de 1’application SocialPass. Le fait qu’iI s’agit d’une coëdition
semble ëtre confirmë par les conditions gënërales SocialPass et SocialScan (cf.
https://www.socialpass.ch/termes-et-conditions/,
version du 17 avril 2021, ch. 1). En vertu du ch. 3 de
13/62

0
la dëclaration de confidentialitë – ëgalement disponible sur Ie site web1 – NewCom4U Särl est l’unique
sociëtë responsable du traitement et maTtre du fichier.
De surcroTt, et dans l’AppStore et dans le PlayStore, SwissHelios GmbH est mentionnë comme unique
distributeur de SocialPass.
Enfin, dans leur courrier du 26.04.2021, les reprësentants des exploitants de SocialPass font rëfërence
ä plusieurs documents selon lesquels les exploitants de SocialPass ont ëtë mandatë par le canton du
Valais et GastroVaud respectivement. Sur la base de la documentation ä notre disposition, GastroVaud
aurait mandatë SwissHelios Särl alors que le canton du Valais aurait mandatë NewCom4U Särl pour
l’exploitation de SocialPass
2.2.
Composants et fonctions
2.2.1. AperQU
Le systëme SocialPass se base essentiellement sur une application pour les entreprises (SocialScan,
cf. chapitre 2.2.3), une application pour les utilisateurs (SocialPass, cf. chapitre 2.2.4) et une base de
donnëes centrale (cf. chapitre 2.2.5). Un apergu du fonctionnement de SocialPass sous forme d’un
schëma est ä disposition sous https://www.socialpass.ch/comment-cela-fonctionne/ (ëtat au
08.05.2021).
Les exploitants de 1’application
SocialPass ont mis ä disposition du PFPDT la figure 1. Cette figure a
servi de base pour 1’analyse technique. Par la suite, notamment en raison du dëveËoppement de
I'application, I'illustration a ëtë complëtëe.
Pour la collecte des coordonnëes des visiteurs, le systëme SocialPass prëvoit deux possibilitës :
Gräce ä 1’application
SocialPass le visiteur scanne un code-QR imprimë.
L'exploitant de I'ëtablissement accessible au public scanne le code-QR des visiteurs. Le
schëma suivant illustre la deuxiëme possibilitë de collecter les coordonnëes des visiteurs.
1 https://www.socialpass.ch/mentionslegales/
14/62

MIt 2864)A
Schhrs8el
geskhed
BetrIeb
Social&an
Gesicherte Datenbank
Gesicherter
Direktzugang
Information
Instruktion
Gast 2 - n
§ocialPass
Figure 1: Schëma tel que figurant dans Ie document SocialPass-SocialScan
Uebersicht-d.pdf
2,2.2.
Description du processus d’enregistrement
Aprës avoir installë I'application, celle-ci est ouverte et aprës avoir sëlectionnë la langue
appropriëe (allemand, anglais, fran9ais, italien ou espagnol), les eonditions d'utilisation, y
compris la dëclaration de confidentialitë, apparaissent. Celles-ci peuvent ëtre soËt acceptëes
soit rejetëes.
Aprës avoir acceptë les conditions d'utilisation, I'utilisateur doit saisir son numëro de
tëlëphone. Ensuite, un masque d'enregistrement apparait, dans lequel il doit impërativement
indiquer son nom, son prënom et son code postal. II importe peu que les donnëes soient
correctes ou non, ä I'exception du numëro de tëlëphone.
En cliquant sur (service tiers
amëricain). Au cours de ce processus, un code QR est gënërë et stockë sur l’appareil mobile
de l’utilisateur. Cela signifie qu'un visiteur d'un ëtablissement (par exemple d’un restaurant)
peut soit faire scanner ce code QR par le personnel du restaurant (possËbilitë 2), soit scanner
un code QR sur la table (avec le numëro de la table) – processus qui correspond ä la
premiëre possibilitë dëcrite ci-dessus. II est ëgalement possible d’enregistrer des personnes
qui n'ont pas 1’application
SocialPass via la saisie manuelle (cf. chapitre 2.4.1), par exemple
parce qu’elles n'ont pas d’appareil mobile.
Les donnëes sont ensuite cryptëes et transfërëes directement vers une base de donnëes SQL
centrale (Microsoft Azure), qui est hëbergëe par Microsoft en Suisse. Cela permet aux
traceurs autorisës d'accëder directement aux donnëes afin de prëvenir les personnes
potentiellement infectëes
(1)
(2)
(3)
(4)
15/62

0
(5)
Le fait de quitter un ëtablissement (saisi par un autre scan) est ëgalement enregistrë et
transfërë dans Ia base de donnëes.
Processus documentation visites
8
TOb4B
c08yr&##cabcxt
d 6hckß9e
en
Oruanbateurs
natIon
Instruction - Quarantaine
Vlstteur 1
So GirlPass
Vi$tteur8 2 . n
1 o.-i’ !Pass
Trageurs ae contact des
mëdecins cantonaux
Si direct sëcuhtë par
autlrentlficatm
d(utie facteur
Figure 2: Schëma actualisë du mode de fonctionnement de SocialPass
(6)
La figure 2 montre qu'un traceur peut accëder directement aux informations des visiteurs
potentiellement infectës sur la base de donnëes en utilisant une authentification ä deux
facteurs. En outre, les autoritës cantonales ont un accës direct aux donnëes enregistrëes
dans Ia base de donnëes Azure lorsque I'utilisation de I'application SocialPass est rendue
obligatoire par ces autoritës (cf. chapitre 2.2.5.b).
La figure 2 montre ëgalement que l’accës des mëdecins cantonaux aux donnëes diffëre d’un
canton ä un autre. Selon le modële choisi, les exploitants d’ëtablissements accessibles au
public peuvent demander une liste d'informations sous forme de fichier Excel/PDF et la
transmettre aux traceurs ou si les traceurs peuvent accëder directement aux coordonnëes des
visiteurs.
(7)
16/62

0
2.2.3.
Fonctions deSocialScan
Le composant SocËalScan est utilisë par un ëtablissement accessible au public (par exemple un
restaurant) pour enregistrer les coordonnëes des visiteurs et peut ëtre installë sur les pIateformes iOS
et Android.
Lors de I'enregistrement d'un ëtablissement dans SocialScan dans Ie but de crëer un compte, les
donnëes suivantes sont collectëes (les champs obligatoires ëtant marquës par un *) :
«Organisation»*: restaurant, ëvënement, religion, prestations de service, restaurant Berne,
sport, gënëral – simple, famiIIe, chantier de construction, centre de formation, EMS ou
organisation partenaire
Nom*
Adresse*
Code postal*
Ville*
E-Mail*
Tëlëphone*
Nom de la personne responsabËe*
Mot de passe*
L’adresse mail et le mot de passe sont utilisës pour crëer un compte d’utilisateur
Les donnëes des ëtablissements sont traitëes ä deux fins diffërentes. D'une part, lors d'une visite dans
un ëtablissement accessible au public, les coordonnëes des visiteurs sont complëtëes avec les
donnëes portant sur l’ëtablissement, l’ëvënement, etc. puis transmises ä la base de donnëes centrale
aux fins de la collecte des coordonnëes des visiteurs/ä des fins de tra9age (contact tracing). D’autre
part, les donnëes sont transfërëes dans le systëme de gestion de la relation client (Customer
Relationship Management, CRM) de NewCom4U Särl. En fonction de I'abonnement conclu entre les
ëtablissements et les exploitants de SocialPass, ce systëme gëre les processus de paiement pour
I'utilisation de I'application.
2.2.4_
SocialPass : enregistrement et utilisation
SocialPass est le composant utilisë par les clients d'un ëtablissement. L'application est gratuite et peut
ëtre utilisëe sur les appareils iOS et Android
Aprës avoir tëlëchargë le composant SocialPass sur son tëlëphone mobile et acceptë la dëclaration de
confidentialitë (un document intitulë 
consultable sous https://www.socialpass.ch/mentionslegales/; ëtat au 10.05.2021), l’utilisateur doit
17/62

0
indiquer son numëro de portable qui est ensuite vërifië. La vërification se fait via le prestataire amëricain
 (cf. chiffre 2.5.2), toutefois I'utilisateur n’en est pas informë.
L'utilisateur
re9oit un code de vërification par SMS sur le numëro indiquë et procëde ensuite ä
< 1’enregistrement
du client >. A cette fin, iI doit indiquer les donnëes suivantes (les champs obligatoires
ëtant marquës par un *) :
Nom*
Prënom*
Numëro de tëlëphone mobile* (repris du pas prëcëdent)
Code postal*
Date de naissance
Adresse
E-Mail
II convient de noter que la date de naissance constituait un champ obligatoire au dëbut de la procëdure
d’ëtablissement de faits, ce qui a ëtë adaptë au cours de la procëdure.
Ä 1’exception du numëro de tëlëphone (voir ci-dessus), les donnëes enregistrëes par l’utilisateur ne sont
pas vërifiëes. Elles peuvent en outre ëtre adaptëes ä tout moment. Lorsque l’utilisateur veut changer le
numëro de tëlëphone mobile indiquë lors de l’enregistrement, iI re9oit un nouveau code de vërification.
Les coordonnëes collectëes sont sauvegardëes localement sur l’appareil mobile de l’utilisateur.
Une fois l’inscription complëtëe, l’utilisateur dispose d’un code QR qui peut ëtre affichë sur son portable.
11 peut ensuite montrer ce code ä l’exploitant de l’ëtablissement lorsqu’iI accëde audit ëtablissement.
L’expËoitant scanne alors Ie code QR gräce au composant SocialScan.
Le client peut ëgalement scanner lui-mëme, ä I'aide de 1’application SocialPass, un code QR fourni par
I'exploitant de l’ëtablissement accessible au public et I'utiliser pours’enregistrer. 11 convient de noter que
dans cette deuxiëme hypothëse, iI n’est pas possible de vërifier si Ie code QR mis ä disposition par
l’exploitant
de l’ëtablissement
ne renvoie pas ä un contenu dangereux, puisque I'application
ne
demande pas de reconfirmation avant de transmettre les donnëes aprës Ie scan du code QR
Quand Ie code QR de l’utilisateur est lu par un appareil de I'exploitant ou que l’utilisateur scanne Ie code
QR mis ä disposition par I'ëtablissement, les coordonnëes des visiteurs enregistrëes, complëtëes par
les donnëes relatives ä la visite dans I'ëtablissement (« dëtails de prësence dans une organisation »)
sont alors transfërëes dans une base de donnëes SQL (Microsoft Azure, cf. chapitre 2.5.3)
18/62

0
2.2.5. Base de donnëes centralisëe
a.
Gënëralitës
Lors d'une visite, les coordonnëes du visiteur (nom, adresse, email, numëro de tëlëphone, etc.) sont
combinëes avec les donnëes de I'ëtablissement accessible au public (nom, emplacement, table, etc.)
et Ie moment de la visite (checkin / checkout) pour former un ensemble de donnëes. Cet ensemble de
donnëes (coordonnëes du visiteur / donnëes de l’ëtablissement / heures de prësence) est ensuite
transmis de maniëre cryptëe et stockë dans ia base de donnëes centrale d'Azure (Suisse Nord / Zurich).
Les interfaces de programmation API (Application Programming Interfaces) sont utiËisëes pour la
transmission des donnëes
D’une maniëre gënërale, les accës aux API sont protëgës par I'utilisation de jetons de sëcuritë du type
JWT encryptë ä I'aide d’algorithmes AES 256. Les API sont aussi dëployës dans Ie cloud Azure Suisse.
Le tableau suivant rëcapitule, ä titre d’exemple, 1’ensemble des donnëes qui sont transfërëes ä la base
de donnëes centrale en tant que « dëtails de prësence dans une organisation » aux fins de la collecte
des coordonnëes des visiteurs en vertu des dispositions lëgales en vigueur :
PresenceDatal D
Orqanizationl D
LastName
FirstName
PhoneNr
Reservation Date
Field1 Value
C
PostalCode
Canton
Arrival
Departu re
DateOfBirth
Adress
4016282
17800
Doe
John
+41791234567
2021 -01 -28
Table 2
Berne
3003
Berne
2021-01-28 10:32:00.000
2021-01-28 11 :45:00.000
1999-01 -01
Feldeggweg 1
Les dëtails des prësences dans une organisation peuvent ëtre transmises soit par SocialPass ou par
SocialScan, selon Ia variante utiËisëe (cf. chapitre 2.4),
Malgrë les demandes explicites du PFPDT, iI n'a pas ëtë possible d'ëtablir quelles ëtaient les mesures
de protection des donnëes dans Azure et si les donnëes sont stockëes sous forme cryptëe ou non (data
at rest protection).
Les dëtails de prësence dans une organisation sont supprimës aprës 14 jours. Ä cette fin, une täche
planifiëe a ëtë exëcutëe ä I'aide de la fonction ; Ie script fonctionne en continu et supprime
automatiquement, deux fois parjour, les enregistrements de donnëes de plus de 14 jours.
19/62

0
Le stockage des dëtails de prësence dans une organisation transmËses est centralisë, c'est-ä-dire que
Ie stockage desdits dëtails de prësence n’est ni physiquement ni logiquement sëparë, iI n'y a pas de
sëgrëgation (sëparation) des donnëes par canton ou par ëtablissement accessible au public. En
d’autres termes, iI n’y a qu'une seule base de donnëes centrale pour toutes les donnëes relatives aux
visiteurs de tous les ëtablissements participants au systëme SocialPass dans toute Ia Suisse.
b.
Accës des autoritës cantonales aux coordonnëes des clients
11 y a deux possibilitës d'accës aux donnëes centralisëes lors d’un cas d’infection : la remise d’une liste
ä I'autoritë compëtente par l’ëtablissement ou un accës direct par les autoritës en charge de la santë
publique (cantons de Valais et Vaud).
Dans Ia variante « remise d’une liste » l’ëtablissement peut, si les autoritës compëtentes le lui
demandent pour l’identification
des personnes prësentes, tëlëcharger une liste des coordonnëes des
visiteurs pour une përiode donnëe et la mettre ä la disposition de I'autoritë cantonale.
Dans Ia variante < accës direct par les autoritës sanitaires » les autoritës cantonales compëtentes,
comme p.ex. les mëdecins cantonaux, peuvent obtenir un accës direct ä la base de donnëes Azure.
Chaque canton peut, s’iI le souhaite, demander un accës direct sur la base de donnëes centralisëe,
Les mëdecins cantonaux sont alors dans le röle du < power user » qui leur permet de crëer des logins
pour leurs co11aborateurs. Actue11ement (ëtat au 10.05.2021), seuls les autoritës sanitaires des
Cantons de Vaud et Valais ont la possibilitë d’accëder directement aux bases de donnëes
centralisëes. Par le biais de cet accës direct ä la base de donnëes, les autoritës cantonales peuvent
effectuer de multiples traitements de donnëes.
20/62

0
Le schëma suivant illustre les fonctions que les autoritës sanitaires peuvent utiliser
Add 1 Under
thr+eü! User
Fxport tn CSV
Elpert to End
14)(lülleBser
rldaH#881
API
addy=
#_______
,...N,_,,.„=H.,nh_,
Figure 3: Backoffice Health Authority – Diagramme logique du flux de donnëes, dans : Rapport technique
(Document [DD, p. 17
Le systëme SocialPass met ä disposition plusieurs fonctions pour traiter les donnëes des visiteurs
Ainsi, les autoritës sanitaires disposent des fonctions suivantes en fonction de leurs permissions :
• Gestion des collaborateurs (cf. Health Autority dans le schëma ci-dessus)
• Chargement du fichier des cas positifs (cf. Upload positive cases dans le schëma ci-dessus)
• Recherche (cf. Search dans le schëma ci-dessus)
• Total des cas par organisation (cf. Total cases by organization dans le schëma ci-dessus)
21 /62

0
La premiëre fonction est accessible aux personnes disposant d'un droit d’administrer les
collaborateurs. TroËs types de droits sont disponibles :
• Primary (permet d’administrer)
' Power (permet d’importer/exporter)
• Normal (permet de visualiser)
Le type Primary est dëfini par l’ëquipe de support de SocialPass. En gënëral c’est le compte du
Mëdecin Cantonal. Un canton spëcifique est indiquë pour le Primary. Le type Power et Normal est
dëfini par l’utilisateur de type Primary. Le canton ne peut ëtre changë, ainsi, par exemple, si un
Primary est rattachë au canton de Vaud, le Power et Ie Normal le seront ëgatement. L’ancrage ä un
canton limite par la suite la capacitë de la recherche ä ce seul canton. 11 en dëcoule, par exemple, que
les collaborateurs du canton de Vaud n’auront pas accës aux donnëes des personnes rësidantes
dans le canton du Valais
Selon les informations soumises par les reprësentants de SocialPass, aucune autre partie que les
certains exploitants dëterminës en amont et les autoritës sanitaires n'ont accës ä la base de donnëes
centralisëe.
Les reprësentants lëgaux n’ont fourni aucune information ä propos de I'enregistrement des accës, bien
que le PFPDT leur ait adressë plusieurs questions ä ce sujet. Ainsi, sur la base de la documentation
disponible, le PFPDT n'a pas pu procëder ä une conclusion claire en la matiëre
La deuxiëme fonction (Upload positive cases) permet de charger Ia liste des cas ayant ëtë testë
positifs au Covid-19.
La troisiëme fonction (Search) permet de rechercher des prësences dans des organisations
(ëtablissements accessibles au public) en utilisant plusieurs filtres. Lors de requëtes diffërents champs
de donnëes peuvent ëtre utilisës (voir Ia capture d'ëcran ci-dessous). Ce mode de recherche permet
de spëcifiquement rechercher des personnes individuelles (nom, prënom), des numëros de tëlëphone
ou des codes postaux. La recherche peut ëtre limitëe dans le temps et/ou ä des ëtablissements
spëcifiques (filtre). Les requëtes permettent d'effectuer des recherches avec des caractëres
gënëriques, ce qui permet d'obtenir un grand nombre de rësultats.
22/62

0
1:tt FreIeto
OFhH
A+#n\Cal6
611B
olW'ü14tßoonKyuj+a
CxlgbaTUI EHud
aIMunab+bb
QmnHrlIHuB•
OBHH+L88tHHBe
nHnBl ruHen LHlbUe
GnHI
aHh 8
!!
!:
tHBüIF
::
nun Nb 8
::
AdHnCab
lin
&IIII
nHI
OWÜBIB
ugjll
menGe
8118
nun
HIn ,
@96srßn8
vbIll
Aal#Bah
no
hIhi
Uh
Hin
UB63an6 VH
AdBHQBglü 1180 nHhöße
Re4LA
aRNe8aß UHI
Figure 4: Options de recherches pour les autoritës sanitaires, dans
Ardfd
OBeRn
SU 8
One/}hB 8 Daß/n
TaU 3
HaftEn
26artig9
bbk 2
KiafiBot
a&nrtkSB
TöBb FI
KIaraBe
aKUPPBIR
abb 6
Kafit+8
e&w169p
Rapport technique (Document [DD, p. 75
La quatriëme fonction (Total cases by organization) permet de retrouver les organisations
(ëtablissements accessibles au public) dans lequel des cas positifs ont effectuë une visite. Les options
de recherche suivantes sont alors disponibles :
• Voir les cas positifs
• Exporter Ia liste des cas positifs, y compris les personnes en contact direct avec la personne infectëe
• Exporter Ia liste des personnes ayant frëquentë le mëme ëtablissement que les cas positifs
• Exporter uniquement les numëros de tëlëphone des personnes en contact direct avec les cas positifs
(option spëcifique au canton du Valais).
Ä partir de la recherche des cas positifs dans les organisations on peut obtenir l’identification de ces
cas. Ä partir de la recherche prëcëdente on peut obtenir Ia liste des personnes ayant ëtë en contact
direct avec les cas positifs. Pour cette option de recherche, la restriction sur le canton ne s’applique
pas. Tous les contacts du cas positif sont identifiës.
2.3.
But de la collecte des donnëes
Selon Ie ch. 7 de la dëclaration de confidentialitë2, qui trouve son fondement dans l’Ordonnance Covid-
19 situation particuliëre, la collecte des donnëes se fait uniquement dans Ie but de les transmettre aux
autoritës publiques en cas d'infection confirmëe de COVID-19 au sein de l’ëtablissement accessible au
public,
2 Document < SocialPass - SocialScan et la protection des donnëes », https://www.socialpass.ch/mentionslegales/, ëtat au
10,05.2021 ; identique au document < Privacy Policy - SocialPass et SocialScan », annexe n' 1 au courrier du 26.04.2021
23/62

0
2.4.
Description des diffërents modes de fonctionnement
2.4.1. SocialScan : saisie manuelle (enregistrement des clients rëguliers)
Lorsque l’exploitant de l’ëtablissement accessible au public enregistre les coordonnëes du client
manuellement (saisie manuelle), le client devrait, en principe, pouvoir choisird'ajouter ses donnëes ä la
liste des , d'imprimer un code QR ou de continuer sans rien faire. En pratique
toutefois, le choix entre ces diffërences options appartient ä I'utilisateur de SocialScan. En effet, c'est
l’utilisateur de SocialScan, c'est-ä-dire I'exploitant de l’ëtablissement accessible au public qui dispose
de l’appareil sur lequel SocialScan a ëtë tëlëchargë.
Si le choix porte sur I'inscription sur de la liste des clients rëguliers, les donnëes sont stockëes
localement sur I'appareil de l’utilisateur de SocialScan, c'est-ä-dire de l’exploitant de l’ëtablissement
accessible au public. Les coordonnëes peuvent ensuite ëtre rëutilisëes lors d’une nouvelle visite via la
fonction . Lorsque la fonction « saisie manuelle > est choisie, la liste sur laquelle
figure toutes les coordonnëes des « clients rëguliers » enregistrës s’affiche lorsqu’est sëlectionnëe la
fonction < choisir un client ». L'utilisateur de SocialScan peut accëder ä cette liste ä tout moment. Toutes
les coordonnëes s’affichent alors en texte clair. Sur la base des informations soumises au PFPDT
aucune fonction permettant de supprimer ä nouveau les donnëes enregistrëes ne semble exister. En
outre, aucune information sur la durëe de conservation des donnëes des < clients rëguliers » ne figure
dans la documentation soumise dans le cadre de cette procëdure
La liste des avec
d’autres appareils de I'exploitant de l’ëtablissement accessible au public (p.ex. lorsque l’ëquipe de
service est composëe de plusieurs collaborateurs). L’ensemble des donnëes des < clients rëguliers »
peut ëtre affichëe sous forme d'un code QR. Ce code QR peut ensuite ëtre lu directement ä partir d'un
autre appareil (importation) ou imprimë (puis lu par les appareils des diffërents collaborateurs)
Enftn, iI convient de noter que lorsque les coordonnëes d’un < client rëgulier » sont enregistrëes, le
numëro de tëlëphone de ce client n'est pas vërifië – contrairement ä ce qui est prëvu lors du
tëlëchargement de 1’application SocialPass
Les deux captures d’ëcran suivantes montrent Ie point de menu pour ta saisie manuelle des donnëes
des dans Socialscan et les donnëes ä saisir et ä transmettre
24/62

0
A- SocialScan
aHH
+
Soumettre les informations
ahoi.sir un client
16b
EntFëe 0
Srxtie. O
h&nl
0
0
INFOS CLIENTS
®IEp
Nam-
Dëpan
rna:1ITh
Forrctions
S:9
Caltl€ikr
Prëirolll-
@1
tkrnandu la bste
MobIle*
Code po stal1
Adresse
<>R Ctxle rnultipk
Date de naissanc:e
FIFa:1
Version: 6.3
§uppört
NFOS-EMS
_• - Date
W 08.01.2021
Heu ; e
10:37
0
Figure 5 : ëcrans de SocialScan. dans : Rapport technique (Document [DD, p. 61 ss.
Ä noter : la fonction ëtait appelëe dans Ia version 6.3 et a ëtë renommëe < saisie
manuelle > dans Ia version actuelle.
25/62

0
2.4.2_
Stockage des numëros de tëlëphone mobile issus du processus d'enregistrement
Au cours du processus d'enregistrement, le numëro de tëlëphone mobile est traitë dans Ie but de vërifier
I'authenticitë du numëro indiquë. Avant de dëclencher la vërification par SMS gräce aux services Twilio,
iI est vërifië si le numëro de tëlëphone indiquë a dëjä ëtë utilisë une fois pour I'inscription dans
SocialPass. Ä cette fin, tous les numëros de tëlëphone mobile utilisës prëcëdemment sont stockës de
maniëre centralisëe sur Microsoft Azure. Lorsqu’un nouvel enregistrement est effectuë, ces donnëes
sont interrogëes
11 n'y a aucune indication que tes numëros de tëlëphone sont supprimës aprës une certaine përiode de
temps. En outre, I'utilisateur n'est pas informë de ce stockage permanent lors de la procëdure
d'enregistrement. II n'y a pas non plus d'indication sur la maniëre dont I'utilisateur peut faire supprimer
ces donnëes.
II est important de noter que le traitement du numëro de tëlëphone rëpond ä deux objectifs diffërents
D'une part, le numëro de tëlëphone est traitë afin de procëder ä sa vërification de ce numëro par l’envoi
d’un SMS et, d'autre part, pour rëpondre aux exigences lëgales qui fixent que la collecte du numëro de
tëlëphone est obligatoire afin de permettre le tragage (contact tracing). Ce sous-chapitre se penche sur
Ie traitement des donnëes tel que prëvu par Ie premier objectif dëcrit ci-dessus.
2.5.
Services de tiers
2.5.1.
Infomaniak
Le site www.socialpass.ch sert principalement de portail d'information pour la plateforme SocialPass et
est hëbergë par Infomaniak en Suisse. Infomaniak est un hëbergeur suisse dont les centres de donnëes
sont situës exclusivement en Suisse. Ä I'origine, le site www.socialpass.ch ëtait hëbergë par un
fournisseur en France. Aprës Ie premier audit de la sociëtë Navixia SA en novembre 2020,
l’hëbergement a ëtë confië ä Infomaniak en Suisse.
Le fonctionnement du site web et le traitement des donnëes associë ne sont pas examinës dans le
cadre de cette enquëte. Sur la base des informations ä notre disposition, iI n’y a pas d'ëchange de
donnëes entre Ie site web et les applications SocialPass ou SocialScan ; au moment de la prësente
enquëte, le site web est uniquement utilisë ä des fins d'Ënformation.
2.5.2.
Twilio
Twilio est une entreprise amëricaine basëe ä San Francisco, aux Ëtats-Unis. EIle exploite une
plateforme de communication en nuage en tant que « Platform as a Service >.
26/62

0
Aprës I'enregistrement
initial auprës de SocialPass, Twilio permet I'envoi du SMS aux utilisateurs de
SocialPass. En recevant Ie SMS, la validitë du numëro du client est confirmëe. Ä la fin du processus de
vërification, une clef unique est renvoyëe par ce service si le processus a pu ëtre achevë correctement,
Force est de constater que lors de l’utilisation du service Twilio des donnëes personnelles au sens de
la LPD, notamment les numëros de tëlëphone des visËteurs, son transfërëes aux US. Toutefois, sur la
base de la documentation ä notre disposition, nous constatons que les opërateurs de SocialPass n'ont
pas vërifië si des mesures autres que celles prëvues dans les clauses contractuelles ëtaient nëcessaires
et, le cas ëchëant, si elles avaient ëtë mises en place.
La finalitë de la collecte et du traitement des numëros de tëlëphone ne ressort pas clairement des
documents soumis au PFPDT ; toutefois, sur la base des informations
dont nous disposons, ces
donnëes ne semblent pas ëtre traitëes en tant que coordonnëes, mais sont traitëes afin de vërifier
l’authenticitë du numëro de tëlëphone indiquë.
2.5.3. Microsoft Azure (base de donnëes SQL)
Une base de donnëes Azure SQL de Microsoft, hëbergëe en Suisse, est utilisëe pour stocker les
donnëes tel que dëcrit ci-dessus. Les rapports de test [B] et [Cl qui nous ont ëtë fournis ne concernent
que le composant SocialScan pour Android et iOS. Ils ne contiennent aucune information sur le
composant SocialPass ou les services de fournisseurs tiers, tels que Twilio ou Microsoft Azure. Afin de
permettre au PFPDT de mieux ëvaluer le traitement en termes de sëcuritë et de protection des donnëes,
des rëponses spëcifiques supplëmentaires ont ëtë demandëes ä SwissHelios dans Ie document [K]
Dans ce contexte, la question a ëtë posëe de savoir si Azure ëtait configurë conformëment ä la Baseline,
par exemple. Cette question est restëe sans rëponse jusqu’ä ce jour. Le document [1] a ëtë soumis ä
titre d'information. Toutefois, iI ne contient aucune information sur les mesures prises pour sëcuriser le
systëme ni sur la mise en @uvre effective et le contröle de ces mesures. Dans la rëponse (4-c) du
document [H], les exploitants de SocialPass expliquent que la fonction d’audit est activëe sur Azure, qui
enregistre les accës ä la base de donnëes. EIle prëcise ensuite que I'infrastructure AZURE dispose de
toutes les fonctions de sëcuritë, de journalisation et de tragage. II n'est pas expliquë si et comment ceux-
ci sont utilisës et donc activës. Dans ce cadre se pose ëgalement la question de savoir si des
identificateurs et/ou d'autres donnëes personnelles ont ëtë enregistrës dans Azure en plus des donnëes
des visiteurs/clients (=prësence) et si oui, lesquelles.
2.6.
Information et droits des personnes concernëes
2.6.1. Information des utilisateurs
Au cours de la procëdure d'ëtablissement des faits, la dëclaration de protection des donnëes et d'autres
informations publiquement accessibles,
ä savoir les informations disponibles sur Ie site web
www.socialpass.ch, ont ëtë considërablement modifiëes. Actuellement (ëtat au 10.05.2021), tant les
27/62

0
liens dans I'AppStore (Apple/iOS), dans le PlayStore (Google/Android) que dans les applications
SocialPass et SociaËScan
renvoient ä la dëclaration de protection
des donnëes sur Ie site
www.socialpass.ch/mentionslegales/, ce qui ëtait encore incohërent au moment de I'ouverture de la
procëdure.
2.6.2. Droits des personnesconcemëes
a.
Exercice du droit d’accës
Le document « SocialPass – SocËalScan et la protection des donnëes »3, accessibles via I'application,
les AppStores et Ie site web sous le titre < Protection des donnëes », indique une adresse de contact
pour les utilisateurs (info@socialpass.ch; ëtat au 10.05.2021 )
En outre, la dëclaration
de protection
des donnëes contient des informations
sur les droits des
personnes concernëes (cf. ch. 6).
b.
Exercice du droit ä l’effacement des donnëes
L’effacement se fera de fa9on automatisëe aprës la durëe de conservation de 14 jours prëvue par
I'Ordonnance Covid-19 situation particuliëre
Par contre, lorsque la fonction (cf. chapitre 2.4.1) est utilisëe, les coordonnëes des
< clients rëguliers
> restent enregistrëes
sur l’appareil
de l’ëtablissement.
Sur la base de la
documentation soumise au PFPDT, aucune possibilitë d’effacer les donnëes des 
des appareils des ëtablissements accessibles au public ne semble avoir ëtë prëvue par les exploitants
de SocialPass.
Aucune information n'est disponible sur la question de savoir si une sollicitation ä 1’adresse des
utilisateurs de supprimer I'application, et donc toutes les donnëes personnelles dëtenues sur les
appareils, est prëvue lorsque les dispositions pertinentes fondëes surl’Ordonnance COVI D-19 Situation
particuliëre ne seront plus en vigueur,
2.7.
Aspects de sëcuritë des donnëes
2.7.1. Organisation de la sëcuritë de 1’information
Le PFPDT a demandë aux opërateurs de I'application, au moyen d'un questionnaire, comment les
responsabilitës en matiëre de sëcuritë de I'information et de protection des donnëes sont dëfinies,
documentëes et attribuëes entre les deux exploitants de 1’application. Dans leur rëponse ä ce
3 https://www.socialpass.ch/mentionslegales/
28/62

0
questionnaire technique, les exploitants de I'application ont indiquë que la rëpartition des responsabilitës
en matiëre de sëcuritë de I'information et de protection des donnëes n’a pas pu ëtre fixëe (ni par oral ni
par ëcrit), notamment en raison des modifications constantes de I'application au niveau cantonal ainsi
qu’en raison des dëveloppements rapides, mais que peu prëvisibles de la pandëmie.
2.7.2.
Login avec double-authentification
Sur la base des informations soumises au PFPDT, iI n'est pas clair si et, le cas ëchëant, quels
composants du systëme de SocialPass sont sëcurisës au moyen d'une authentification ä deux
facteurs.
2.7.3. Identifiants de l’utilisateur
Selon le chapitre [D] "8.11 - Device - Structure des donnëes", diffërents identifiants d'utilisateur sont
utilisës. Outre le numëro de tëlëphone, iI convient de mentionner explicitement I'utilisation de I'IMEI
(International Mobile Equipment EntËty, un numëro de sërie ä quinze chiffres unËque au monde de
I'appareil) et d'un numëro d'utilisateur unique UID (Unique ID) de Google Firebase. Aucune autre
donnëe pseudonymisëe servant ä identifier de maniëre unique les personnes concernëes n'a ëtë
mentionnëe, mëme aprës des demandes explicites du PFPDT.
2.7.4. Gëolocalisation
SocialPass n’utilise pas la gëolocalisation
2.8.
Analyse de 1’audit de Navixia SA
Les composants et < SocialScan » ont fait I'objet d'un test de vulnërabilitë par NavixËa
SA, pour le compte de GastroVaud,
aux dates suivantes. Cela vaut pour les systëmes d'exploitation
iOS et Android.
Date
Processus
18 mars 2021
Rapport, y compris Management Summary v.1.2
Test du cryptage mis en oeuvre
Rapport, y compris Management Summary v.1.1
Vërifications 2 et 3
12 au 18 mars 2021
7 dëcembre 2020
4 dëcembre 2020
16 au 18 novembre 2020
Kick-Off et test
Selon le rapport « Analyse de sëcuritë (recheck) Applications SocialPass & SocialScan v. 1.2 > datë du
18 mars 2021, tous les ëlëments des applications susceptibles d'ëtre pertinents pour la sëcuritë ont ëtë
29/62

0
examinës.
Cela
comprend le stockage
des
donnëes,
la confidentiatitë, la cryptographie,
I'authentification, la communication rëseau et les paramëtres de construction.
Pour analyser les applications mobiles, Navixia SA suit une mëthodologie basëe sur I'ëvaluation des
risques OWASP. Cette approche suit un processus structurë et rend tes rësultats obtenus comparables
entre eux. Ä cette fin, pour chaque ëlëment identifië, la vulnërabilitë est dëcrite et son degrë de risque
est cartographië sur la base du systëme normalisë CVSS (Common Vulnerability Scoring System). Les
rësultats sont ëvaluës selon les critëres suivants :
•
Exploitabilitë : les vecteurs d'accës, la complexitë de I'accës et I'authentification ëvaluent comment
un attaquant peut accëder ä une vulnërabilitë et quelles conditions supplëmentaires, le cas ëchëant,
doivent ëtre remplies pourqu'elle soit exploitëe.
•
Implications
: Les indices de protection des donnëes, d'intëgritë du systëme et de disponibilitë
mesurent la maniëre dont une vulnërabilitë peut avoir un impact direct sur I'infrastructure
informatique une fois exploitëe.
Dans le CVSS, le score total d'une vulnërabilitë rësulte de la combinaison d'une sërie d'ëvaluations
isolëes d'aspects indËviduels (mëtriques), en tenant compte des pondërations enregistrëes dans la
formule de calcul.
Les indices de mesure ä cet effet sont indiquës ci-dessous avec les valeurs attribuëes correspondantes,
Cet indice ëvalue Ie niveau d'autorisation qu'un attaquant doit avoir afin d'exploiter avec succës la
vulnërabilitë.
Haut:
L'attaquant dispose de privilëges qui lui donnent accës ä des röles administratifs
importants.
L’attaquant dispose de privilëges d'utilisateur de base qui peuvent affecter les
paramëtres et les fichiers d'un utilisateur.
L'attaquant n'a pas besoin d’ëtre authentifië
Moyen :
Faible:
lci, I'ëvaluation est basëe sur I'impact d'une vulnërabilitë sur la confidentialitë des donnëes traitëes.
Confidentialitë
Haut:
11 y a une perte totale de confidentialitë et un attaquant obtËent I'accës ä toutes les
ressources du composant affectë.
Un attaquant peut accëder ä certaines donnëes.
II existe un faible risque d'accës aux donnëes au sein du composant concernë.
Moyen :
Faible:
30/62

0
Cet indice dëcrit Ë'impact d'une vulnërabilitë sur I'intëgritë du systëme.
Haut:
11 en rësulte une perte totale d'intëgritë. Par exemple, l’attaquant peut modifier
n'importe quel fichier (ou ensemble de fichiers).
Moyen :
Faible:
La modification de donnëes est possible dans une mesure limitëe. Cependant, la
modification des donnëes n'a pas d'impact significatif sur le composant concernë.
11 y a un faible risque de perte d’intëgritë.
Le degrë de danger est ëvaluë dans le rapport de Navixia SA sur la base des ëlëments ci-dessus sur
une ëchelle de O ä 10.
• Score entre 9,0 et 10: critique
• Score entre 7,0 et 8,9: 111:jIt
• Score entre 4,0 et 6,9: ,
• Score entre 0,1 et 3,9: faible
• Score 0: ä titre d’information
Du point de vue du PFPDT, les interprëtations suivantes doivent servir de rëfërence, en fonction de
I'indice d’ëvaluation, afin de prëvenir les risques de violation de la protection des donnëes.
Critique:
Haut;
Cette vulnërabilitë reprësente un risque inacceptable. L’application ne doËt pas ëtre
mise en ligne ; si eIle 1’est dëjä, eIle doit ëtre dësactivëe immëdiatement.
Cette vulnërabilitë doit ëtre corrigëe immëdiatement, ëventuellement dans le cadre
d'un correctif d'urgence. D'autres mesures de minimisation des risques doivent ëtre
envisagëes jusqu'ä ce que le correctif soit en place.
Moyen :
Faible:
Cette vulnërabilitë doit ëtre corrigëe, mëme si eIle entraine des coüts
supplëmentaires (modërës) ou d'autres inconvënients (modërës)
Le correctif peut ëtre inclus dans la planification des versions sur une base rëguliëre.
Par la suite, les conclusions du document < GVD7009 Recheck SocialPass SocialScan_v1.2 » sont
dëcrites.
2. 8. 7.
Interaction avec la plateforme (6.2.6 et 6.3.64)
Actuellement, le serveur ne vërifie pas les mëtacaractëres. Le cross-site scripting (XSS) n'est souvent
que le prëcurseur d'attaques plus graves. Actuellement, aucune vërification des donnëes n’a lieu avant
leur exëcution par le serveur
4 Les chiffres se rëfërent aux chapitres du document [A] < GVD7009_Recheck_SocialPass_SocialScan_v1
.2 >
31 /62

2.8.2. Qualitë du code et packaging (6.3.7)
Comme dëcrit dans le rapport d'audit, un attaquant peut modifier I'APK (paquet Android) afin qu'il
contienne une ancienne version d'une bibliothëque externe sans que cela soit dëtectë par la signature.
Toutefois, si cette ancienne bibliothëque contient des vulnërabiIËtës, l’APK peut ëtre installë sur un
tëlëphone mobile, par exemple, sans briser la signature existante. II est ainsi possible d'exploiter les
failles de sëcuritë des anciennes bibËiothëques.
En outre, les versions intëgrëes des bibIËothëques tierces ont ëtë examinëes au cours de I'audit. 11 a ëtë
constatë que toutes les bibliothëques ne sont pas de la derniëre version. En fait, les bibliothëques tierces
obsolëtes sont souvent affectëes par des failles de sëcuritë.
2.8.3.
Descripteur (7.1)
Le descripteur d'API utilisë par les applications mobiles est accessible au public. Cela permet ä un
attaquant de dëtecter toutes les mëthodes disponibles. D'aprës le rapport, le descripteur d'API n'est
plus visible dans I'environnement de test UAT (User Acceptance Test), mais peut toujours ëtre consultë
en production. Un attaquant peut en tirer des informations pour attaquer I'environnement UAT. Le
problëme ne peut donc ëtre rësolu que si 1’information n'est pas du tout visible.
2.8.4.
Mots de passe stockës en clair (7.1)
Dans le cadre d’interviews, les dëveloppeurs de SocialPass ont confirmë ä Navixia SA que les mots de
passe ne sont plus stockës en texte clair dans la base de donnëes. Cependant, sans accës ä cette base
de donnëes, iI n'a pas ëtë possible pour Navixia de vërifier si les mots de passe sont maËntenant stockës
correctement (salt & hash). Dës lors, le PFPDT part du principe que les dëclarations faites par les
dëveloppeurs dans le rapport sont correctes et que les mots de passe ne sont plus seulement stockës
en texte clair, mais qu'ils sont ëgalement sëcurisës par un Medium Salting.
2.8.5.
Conservation desdonnëes (8.4.1)
La section 8.4.1 mentionne un problëme de conservation des donnëes deI ä une faille de sëcuritë. Selon
Ie rapport d'audit, cela a ëtë rectifië depuis. Or, ce point ne pouvait plus ëtre vërifië par Navixia SA sans
accës ä la base de donnëes.
32/62

0
2.9.
Analyse de 1’audit d’lndusface
Le PFPDT a regu les deux documents suivants par e-mail Ie 1 1 fëvrier 2021 par le reprësentant lëgal
des exploitants de SocialPass
Rapports d’audit
Android Mobile Application Audit Report of Social Scan v1.0.pdf
SHA2 56
D313DCD4B4D8 FBD2C142F7943C65DB4 FF4155F6B474C2F54 35306ADF438F26CC
iOS Mobile Application Audit Report of Social Scan v1 .0. pdf
SHA2 56
C74551665D7B2 2 IAC133DBBEDC31F6EAB2 77FB151879D14237D680117B6A3BD9
Les deux rapports d'audit fournis (Indusface), se rëfërent exclusivement au composant ,
dans les versions pour Android et iOS. Ils ne contiennent aucune information sur le composant
 ou les systëmes back-end sur < Azure ».
os
Përiodes d’essai
Version SocialScan
Mt
- 04. nM}20
r
0.1 MD5
b82a838aa9f430857581f02693ff26co
28. oct. - 03. nov. 2020
V6.2
MD5
ios
OB81B1417BCD6A7CF8360B133632B241
Les conclusions des rapports et < iOS
Mobile Application Audit Report of Social Scan v1.0 > diffërent en fonction des systëmes d'exploitation
Android et iOS
2.9.1 .
Classification
La classification est basëe sur les catëgories ci-dessous
Impact
DescrËption
A vulnerability wherein an attacker might have the ability to execute commands
on the server or retrieve and modify private information
Security issues are defined as a risk that puts the system and / or data related
to the system in immediate danger.
Medium
Findings indicate a more serious security matter that should be remedied
appropriately within a short amount of time.
Findings usually indicate a minor security risk that does not pose immediate or
short-term danger. An observational point in the site, or detection of certain
applications or web servers
An observational point in the site, or detection of certain applications or web
servers
33/62

0
2.9.2.
Rësultats en fonction des catëgories
Les vulnërabilitës dëtectëes sont classëes dans les catëgories suivantes
Android-App
iOS-App
CritËcaË fi
High: 2
Medium: 2
Low: 21
Information:
3
Critica!: f 1
High: 2
Medium: 1
Low: 18
Information: 1
2.9.3. Android et iOS Mobile
Le tableau ci-dessous reflëte les rësultats d'lndusface [B] et [C] pour le composant « SocialScan > pour
les systëmes d'exploitation Android et iOS. Les entrëes marquëes d'un astërisque (*) sont considërëes
par le PFPDT comme pertinentes pour la protection des donnëes. Mëme s'ils sont considërës comme
faibles dans la cËassifËcation des risques, ils peuvent dëvelopper une classification des risques diffërente
ä la suite d'interactions. Ces entrëes relatives ä la protection des donnëes sont analysëes au chapitre
2.9.4
Le PFPDT utilise les notations suivantes comme critëre pour attënuer le risque de violation de la
protection des donnëes
Cette vulnërabilitë reprësente un risque inacceptable. L'application ne doit pas ëtre
mise en Ëigne ; si eIle 1'est dëjä, eIle doit ëtre dësactivëe immëdiatement.
Cette vulnërabilitë doit ëtre corrigëe immëdiatement, ëventuellement dans le cadre
d'un correctif d'urgence. D'autres mesures de minimisation des risques doivent ëtre
envisagëes jusqu'ä ce que le correctif soit en place
Cette vulnërabilitë doit ëtre corrigëe, mëme si cela entraTne des coüts
supplëmentaires (modërës) ou d'autres inconvënients (modërës)
La correction peut ëtre incluse dans la planification des versions ultërieures sur une
base rëguliëre
Tableau 3: Rësultats trouvës dans SocialScan
Vulnërabilitës
Nr.
Catëgorie de
risques
Blind HTML Injection
High
High
Medium
Insecure Direct Object References
Application is Vulnerable To Email Flooding Attack
34/62

0
4*
5*
6*
7*
8*
9*
10
11*
12*
13*
14*
15*
16’
17*
18*
19*
20
21*
22
23
24
25
26
27
Insecure Logging Of The Application (betrifft nur Android)
Application is Vulnerable To Improper Token Management
Application Accepts Special Character As User Input
Valid Account Can Be Brute Forced
Missing API Rate Limiting
Application Does Not Have A Strong Password Policy
Application is Vulnerable To Reverse Engineering
Cleartexttraffic is Set To True (betrifft nur Android)
Application is Vulnerable To Simultaneous Login
Application's Request/Response Reveals Sensitive Information
SSL Pinning Can Be Bypassed
Insecure Data Storage in File System
Insecure Content Security Policy (Csp)/X-Frame-Options
Missing HSTS Header
Information Leakage From Clipboard
Sensitive Data Disclosure in Recent Apps
Default Web Page Found
Application Has Set Insecure Permissions
Programming Language And Version Disclosure
Application Displays Web Server Banner
Using Known Vulnerable Components
Application Works in Rooted Device
Application Runs On Older Platform
Printstacktraceo Function is Used in The Application
lediu
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Low
Information
Information
35/62

0
setAILowFileAccess Enabled
2.9.4. Conclusions de 1’audit Indusface
Le sous-chapitre 2.9.4 rësume les diffërentes constatations du PFPDT comportant un risque de perte
de donnëes, de corruption de donnëes ou de dommages aux donnëes.
a.
Blind HTML tnjection [1]5
L'injection HTML est utilisëe lorsque I'entrëe dans une application n'est pas validëe. Cela permet de
modifier le contenu d'une page web et tous les utilisateurs qui naviguent sur cette page verront le
contenu modifië. Ainsi, sur la page d'enregistrement de SocialScan, un attaquant peut injecter un HTML
Payload (par exemple, une chaTne de code malveillant) dans les champs de donnëes et rëussir ä
I'enregistrer. L'injection HTML est exëcutëe avec succës dans les modëles d'email.
b.
Insecure Direct Object References
[2]
Les rëfërences directes ä des objets non sëcurisëes (IDOR) constituent un problëme de sëcuritë qui se
produit lorsque le dëveloppeur de I'application utilise un pointeur pour accëder directement ä un objet
d'implëmentation interne, mais ne fournit pas de contröles d'accës et/ou de vërifications d'autorisation
supplëmentaires. Un utilisateur de SocialScan est lië ä son numëro d'identification d'utilisateur par I'ID
de I'organisation. L'attaquant, ä son tour, se connecte ä SocialScan et peut simplement modifier I'ID de
I'organisation ä volontë. Cela permet ä I'attaquant d'avoiraccës aux dëtaiËs de I'utilisateur correspondant
(numëro de tëlëphone mobile et mot de passe).
c.
Insecure Logging Of The Application [4]
Dans SocialScan, les donnëes sensibles d'un point de vue technique sont enregistrëes et peuvent
conduire ä des fuites d'informations. Dans SocialScan, les donnëes sensibles teIles que le nom de
I'utiIËsateur
et le mot de passe sont stockëes sans aucune .
d.
Application is Vulnerable To Improper Token Management [5]
Le rapport indique que dans SocialScan, une session reste active mëme aprës la dëconnexion. Cela
signifie qu’une session peut ëtre reprise et rëutilisëe par un autre utilisateur.
5 Les chiffres entre crochets font rëfërence au tableau 3: Rësultats trouvës dans SocialScan, ci-dessus.
36/62

0
e.
Application Accepts Special eharacter As User Input [6]
SocialScan accepte les caractëres spëciaux (>{</ etc.). Cela peut conduire ä I'exëcution d'un code
malveillant,
f.
Valid Account Can Be Brute Forced [7]
Une attaque par force brute (Brute-Force-Attack) est une mëthode d'attaque banale. La thëorie est que
lors d’une teIle attaque, un nombre infini de tentatives sont faites pour deviner un mot de passe. Ä un
moment donnë, le mot de passe correct devrait ëtre devinë. C'est possible avec SocialScan.
g.
Missing API Rate Limiting [8]
Les interfaces d'application dont les limites de ressources et de quotas sont absentes ou mal
implëmentëes offrent aux attaquants la possibilitë de rëaliser des attaques Brute-Force sur des comptes
d'utilisateyrs ou de provoquer un dëni de service. L'exploitatËon de cette vulnërabilitë ne nëcessite
souvent mëme pas d'authentification ; eIle requiert simplement I'envoi simultanë de plusieurs requëtes.
h.
Application Does Not Have A Strong Password Policy [9]
SocialScan n'a pas de politique de mot de passe ou ne I'applique pas correctement. Par exemple, iI est
possible d'utiliser un mot de passe composë d'une seule lettre.
i.
Cleartexttraffic is Set To True [1 11
Selon le rapport d'audit, le trafic de donnëes sur la plateforme Android s'effectue sans cryptage de
transport (SSLfTLS), c'est-ä-dire en texte clair (HTTP).
j.
Application is Vulnerable To Simultaneous Login [1 2]
II est possible d'ouvrËr plusieurs sessions avec les mëmes donnëes d'identification. Cela augmente donc
la surface d'attaque, puisqu'un attaquant peut utiliser de maniëre transparente des donnëes
d'identification valides en mëme temps que I'utilisateur lëgitime.
k.
Application's Request/Response
Reveals Sensitive Information [13]
Toutes les informations sensibles d'un point de vue technique (c'est-ä-dire les donnëes personnelles et
les autres donnëes qui pourraient potentiellement compromettre la sëcuritë des donnëes, par exemple
Ie mot de passe) ne sont pas obscurcies ä I'aide d'une technique appropriëe teIle que le Salting
37/62

0
l.
SSL Pinning Can Be Bypassed [14]
Dans SocialScan, le SSL Pinning impËëmentë peut ëtre contournë en insërant JavaScript au moment
de I'exëcution.
m.
Insecure Data Storage in File System [15]
Les vulnërabilitës du stockage des donnëes surviennent lorsqu'on suppose que les utilisateurs ou les
logiciels malveillants n'ont pas accës au systëme de fichiers d'un appareil mobile et donc aux
informations sensibles contenues dans la mëmoire de I'appareil. II faut donc s’attendre ä ce qu'un
utilisateur malveillant ou un logËciel malveillant puisse avoir accës ä des donnëes sensibles dans
SocialScan. Le rootage ou le jailbreak d'un appareil mobile contourne toute mesure de protection par
cryptage.
n.
Insecure Content Security Policy (Csp)/X-Frame-Options [1 6]
L'en-tëte de rëponse HTTP de X-Frame-Options dans SocialScan peut ëtre utilisë pour spëcifier si un
navigateur est autorisë ou non ä rendre une page dans un , , , ou .
o.
Missing HSTS Header [17]
SocialScan n'utilise pas d'en-tëte HSTS. Cela signifie que les communications non cryptëes via HTTP
sont autorisëes
p.
Information Leakage From Clipboard [1 8]
SocialScan permet de copier-coller ä partir du presse-papiers, notamment le copier-coller de mots de
passe figurant dans Ie presse-papiers.
q.
Sensitive Data Disclosure in Recent Apps [1 9]
Au vu du rapport, aucune prëcaution n’est prise pour empëcher I'utilisation de donnëes sensibles (d’un
point de vue technique) par des applications tierces (par exemple, en mettant en cache des
instantanës d'applications).
r.
Application Has Set Insecure Permissions [21]
II s'est avërë que SocialScan n'avait pas dëfini des droits d'accës, ce qui constitue une menace pour
la sëcuritë pouvant entraTner des fuites de donnëes dans le pire des cas
38/62

0
3. Apprëciation juridique et recommandations
Sur la base des faits ëtablis ci-dessus, notifiës aux parties Ie 20 mai 2021, le PFPDT considëre ce qui
suit (chapitre 3). II tient ä relever que contrairement ä ce que peuvent laisser entendre les documents
soumis par les parties, le PFPDT ne fonde pas ses considërations sur 1’« attestation de conformitë »
d'un audit externe teIle que mentionnëe dans Ie document intitulë < COVID-19 – Dispositifs
d'identification de la clientële dans les ëtablissements de restauration, Procëdure de vërification
technique – 15 octobre 2020 ». En effet, une teIle attestation, bien que mentionnëe dans ledit document
figurant au dossier, n’a pas ëtë soumise au PFPDT au cours de la procëdure d'ëtablissement des faits
3.1.
Röles et responsabilitës
Tel que constatë dans le cadre de l’ëtablissement des faits du 20 mai 2021, les informations quant aux
röles et responsabilitës des parties impliquëes dans la prësente procëdure sont restëes contradictoires
(cf. chapitre 2.1).
Sur la base de la documentation
soumise au PFPDT et des informations
disponibles au public, le
PFPDT constate que les deux sociëtës ont dëcidë d’unir leurs efforts et leurs ressources en vue
d’atteindre un but commun (amëlioration du tragage dans le cadre de la pandëmie du COVID-19) et ont
ainsi dëveloppë le systëme SociaËPass sous forme d'une co-ëdition.
En vertu de 1’art. 3 lit. i LPD on entend par maTtre du fichier la personne privëe (physique ou morale) qui
dëcide du but et du contenu du fichier. Cependant, cette notion reflëte une rëalitë ancienne, qui ne
correspond plus aux besoins d’un monde digitalisë. En effet, cette notion remonte ä une ëpoque oü les
fichiers ëtaient constituës de classeurs et de fiches. La notion est avant tout utilisëe dans Ie but de
dëterminer la personne responsable du traitement. Le PFPDT partage l’opinion de certains auteurs qui
proposent de renoncer ä employer cette notion et proposent que la responsabilitë au sens de la LPD
dëcoule des faits du traitement
de donnëes (cf. RuDIN BEAT, Kommentar
zu Art. 3 DSG, N 43, in:
BaerËswyl/Pärli (Hrsg.), Stämpflis Handkommentar zum DSG, 2015).
Force est de constater que les sociëtës NewCom4U Särl et SwissHelios Särl ont dëveloppë le systëme
SocialPass ensemble, elles ont dëcidë du but et du contenu du fichier ainsi que des droits d’accës ä ce
fichier et ce sont elles qui assurent les divers traitements des donnëes. Elles doËvent dës lors ëtre
considërëes toutes les deux maTtres du fichier au sens de la LPD.
La qualitë de maTtre de fichier doit cependant ëtre distinguëe de celle de mandataire au sens de I'art. 10a
LPD. Trois constellations diffërentes sont possibles en pratique : Ie mandant peut ëgalement ëtre maTtre
du fichier, le mandant et le mandataire peuvent ëtre maTtres communs du fichier ou alors le mandataire
peut ëtre considërë maTtre du fichËer, notamment lorsqu'il traite des donnëes pour le compte de son
client (cf. RosENTHAL DAVID/JÖHRI YvoNNE, Kommentar zu Art. 10a DSG, N 19, in Rosenthal/Jöhri
(Hrsg.), Handkommentar zum Datenschutzgesetz sowie weiteren, ausgewählten Bestimmungen, 2008).
39/62

0
Dans Ie cas d'espëce, les dispositions lëgales pertinentes octroient une certaine marge de manmuvre
aux exploitants d'ëtablissements accessibles au public. En effet, le ch. 4.3. de I'annexe 1 de
l’Ordonnance COVID-19 situation particuliëre fixe uniquement que dans le cadre des plans de protection
< les coordonnëes peuvent ëtre collectëes ä l’aide de systëmes de gestion des rëservations ou des
membres, ou encore au moyen de formulaires de contact ». Aucune disposition fëdërale ne vient
prëciser quels systëmes de gestion doivent ëtre privilëgiës. Les deux sociëtës ont donc proposë une
solution numërique afin d'amëliorer le tragage dans le cadre de la pandëmie du COViD-19 (cf. chapitre
1.2). Ce faisant, elles ont proposë un traitement de donnëes ä leurs clients respectifs. En crëant le
systëme SocialPass, elles ont dëcidë du but et du contenu du fichier ainsi que des droits d’accës ä ce
fichier et ce sont elles qui assurent les divers traitements des donnëes. Ainsi, iI dëcoule des
constatations du PFPDT que dans Ie cas d’espëce, les mandataires communs que sont les sociëtës
NewCom4U Särl et SwissHelios Särl doivent ëtre considërës maTtre du fichier au sens de 1’art. 3 lit. i
LPD
Dës lors, la question de savoir qui est Ie mandant, et s'il existe, le cas ëchëant, plusieurs mandants (les
gouvernements
des cantons respectifs, les restaurateurs
pris individuellement,
la faTtiëre des
restaurateurs vaudois) peut rester ouverte.
Le maTtre du fichier est responsable de respecter le cadre lëgal lors de tout traitement de donnëes et
de garantir les droits aux personnes concernëes tels que consacrës dans la LPD (cf. RuDIN, Art. 3 DSG,
N 49 s. et RosENTHAL, Art. 10a DSG, N 22). Le maTtre du fichier est avant tout responsable de faire
suite aux ëventuelles demandes d’accës des personnes concernëes (art. 8 LPD).
II dëcoule de ce qui prëcëde que les sociëtës NewCom4U Särl et SwissHelios Särl ont la qualitë de
maitre de fichier au sens de 1’art. 3 lit. i LPD. Dës lors, iI leurincombe de respecter les obligations lëgales
prëvues par la LPD, la LEp et l’Ordonnance COVID-19 situation particuliëre. En vertu de I'art. 4 al. 4
LPD la collecte de donnëes personnelles, et en particulier les finalitës du traitement desdites donnëes,
doivent ëtre reconnaissables pour la personne concernëe (principe de transparence). Le respect du
principe de transparence permet en effet aux personnes d’exercer leur droit d'accës. Etant donnë que
les indications dans les diffërents documents sont contradictoires dans la mesure oü certains documents
mentionnent les deux sociëtës tandis que d’autres ne mentionnent que l’une des deux sociëtës en tant
que maTtre du fichier, le PFPDT constate une violation du principe de transparence tel que consacrë ä
1’art. 4 al. 4 LPD. En effet, en l’ëtat actuel, les personnes concernëes ne sont pas en mesure de
dëterminer avec certitude quelle personne morale traite leurs donnëes et ä qui, le cas ëchëant, elles
devraient adresser une demande d’accës
40/62

0
(1) Recommandation concernant les röles et responsabilitës
Les socËëtës NewCom4U Särl et SwissHelios Särl doivent uniformiser tous les
documents (site web, appstores et app) afin de respecter leurs obligations
lëgales en tant que maTtres du fichier au sens de 1’art. 3 lit. i LPD
3.2.
Banque de donnëes centralisëe
3.2.1.
Banque de donnëes centralisëe stricto sensu
La collecte des coordonnëes des visiteurs (nom, prënom, numëro de tëlëphone, NPA) trouve son
fondement dans I'art. 5 de l’Ordonnance COViD-19 situation particuliëre, qui oblige les exploitants
d'ëtablissements accessibles au public de collecter lesdites coordonnëes. Cette disposition prëvoit
notamment que les exploitants collectent les coordonnëes des visiteurs et les transmettent aux autoritës
cantonales sur demande, notamment aux fins d’identification et d’information des personnes qui se
trouvaient dans l’ëtablissement
au mëme moment qu’une personne infectëe et qui sont dës lors
prësumëes infectëes au sens de 1’art. 33 LEp. Les coordonnëes doivent impërativement ëtre dëtruites
aprës 14 jours.
Selon Ie ch. 4.5. de l’annexe 1 de l’Ordonnance COVI D-19 situation partËculiëre, iI incombe ä l’exploitant
de garantir la confidentialitë des coordonnëes qu’iI collecte ainsi que la sëcuritë des donnëes,
notamment durant leur conservation. Ainsi, en vertu des diverses dispositions applicables, iI a ëtë prëvu
que les coordonnëes collectëes restent chez les exploitants respectifs. Ce n'est qu'en cas d'infection
dans un ëtablissement dëterminë que les autoritës cantonales doËvent avoir accës aux coordonnëes
des visiteurs de l’ëtablissement concernë. En d’autres termes, iI a ëtë prëvu que les exploitants des
ëtablissements gardent le contröle sur les coordonnëes qu’ils ont collectëes. La disposition fëdërale ne
prëvoit pas d’accës direct ä toutes les coordonnëes collectëes dans tous les restaurants d’un mëme
canton
SocialPass doit ëtre considërë en tant que systëme de gestion tel que prëvu au ch. 4.3. de I'annexe 1
de l’Ordonnance COVI D-19 situation particuliëre. En effet, cette disposition fixe que < les coordonnëes
peuvent ëtre collectëes ä l’aide de systëmes de gestion des rëservations ou des membres, ou encore
au moyen de formulaires de contact ».
Ä la lumiëre de la LPD, les deux sociëtës SwissHelios Särl et NewCom4U Särl doivent ëtre considërëes
des tiers au sens de 1’art. 10a LPD. II dëcoule de cette constatation que le systëme SocialPass ne
devrait que permettre les traitements de donnëes que Ie mandant serait en droit d'effectuer lui-mëme,
c’est-ä-dire que le systëme SocialPass, afin de tomber sous la dëfinition du ch. 4.3. de l’annexe 1 de
l’Ordonnance COVID-19 situation particuliëre, ne devrait que permettre d'effectuer les traitements tels
que prëvus dans l’Ordonnance COVID-19 situation particuliëre
41 /62

0
Cela ëtant, iI convient de distinguer deux questions diffërentes qu'il convient d'analyser sëparëment par
la suite.
Dans le cadre de ce premier sous-chapitre, iI convient de se pencher sur la question de savoir si le
cadre lëgal pertinent permet la mise en place d’une base de donnëes centralisëe. Si le cadre lëgal
fëdëral permet en effet la mise en place d’une base de donnëes centralisëe, se pose alors la question
de savoir si dans Ie cas d’espëce, des mesures appropriëes ont ëtë mises en place afin de rëpondre
aux exigences tenant ä la sëcuritë de donnëes sensibles (cf. art. 7 LPD) et aux exigences lëgales en
matiëre de protection des donnëes (notamment le principe de la proportionnalitë).
Le ch. 4 de I'annexe 1 de I'Ordonnance Covid-19 situation particuliëre qui fixe les dëtails de la collecte
des coordonnëes n’apporte pas de prëcisions quant aux systëmes de gestion des rëservations qui
peuvent ëtre utilisës pour la collecte (cf. ch. 4.3). Le Rapport explicatif concernant 1’ordonnance COVID-
19 situation particuliëre (y inclus grandes manifestations) du 26 mai 2021 n’apporte pas plus de
prëcisions quant ä cette question.
Les dispositions pertinentes se contentent de fixer que de tels systëmes peuvent ëtre utilisës et que les
exploitants ou les organisateurs doivent garantir la confidentialitë des coordonnëes qu’ils collectent et
la sëcuritë des donnëes, notamment durant leur conservation (cf. ch. 4.6.).
Sur la base de ces dispositions laissant une marge de man@uvre aux exploitants dans le choix du
systëme de gestion des rëservations ou des membres, le PFPDT conclut que l’Ordonnance COVID-19
situation particuliëre n’exclut pas, par principe, que les exploitants d’ëtablissements accessibles au
public utilisent des systëmes de gestion des rëservations qui impliquent un enregistrement des donnëes
centralisë. Toutefois, cet enregistrement centralisë ne sera conforme aux exigences lëgales uniquement
si les principes de la protection des donnëes sont respectës et des mesures de sëcuritë appropriëes
sont mises en place en amont (cf. ch. 4.6. Ordonnance COVID-19 situation particuliëre et art. 7 LPD)
Le PFPDT retient dës lors que I'enregistrement des coordonnëes collectëes dans une base de donnëes
centralisëe teIle que prëvue par le systëme SocialPass est conforme au cadre lëgal ä condition que :
les principes gënëraux de la loi sur la protection des donnëes selon I'art. 4 ss. LPD sont
respectës ;
des mesures de sëcuritë appropriëes aient ëtë mises en place en amont, conformëment ä 1’art,
7 LPD en relation avec les art. 8 et 9 OLPD, en particulier l’art. 9 al. 1 let. g OLPD (pour une
analyse des mesures de sëcuritë mises en place, cf. chapitre 3.7).
Dans un deuxiëme temps, iI convient dës lors d’analyser la question de savoir si la solution d'une base
de donnëes centraIËsëes est ëgalement conforme au cadre juridique dans sa forme concrëte,
42/62

0
3.2.2. Divers droits d’accës ä la base de donnëe centralisëe /fonctions de filtres
Dans le cadre de ses analyses, le PFPDT a constatë que le fonctionnement du systëme SocialPass
impliquait I'existence d’une base de donnëes centralisëe (cf. chapitre 3.2.1) qui offre plusieurs options
de recherches ciblëes (p.ex. les personnes ayant accës ä cette base de donnëes peuvent rechercher
toutes les personnes s’appelant Laure ou Christophe ayant visËtë n’importe quel ëtablissement public
dans le canton du Valais au long des 14 derniers jours)
Force est de constater que le droit d’accës direct ä la base de donnëes centralisëe octroyë aux autoritës
cantonales vaudoises et valaisannes, y compris les diffërentes options de recherches ciblëes, peut
conduire ä la crëation de profils de personnalitë au sens de 1’art. 3 lit. d LPD. En effet, en fonction des
ëtabIËssements accessibles au public visitës (p.ex. une maison close) et/ou en raison des personnes
rencontrëes lors de ces visites (p.ex. un visiteur rencontre un avocat spëcialisë en droit pënal), les
donnëes ainsi assemblëes peuvent permettre d’apprëcier les caractëristiques essentielles de la
personnalitë des personnes concernëes.
Au regard des dispositions lëgales pertinentes du droit fëdëral, ces multiples possibilitës de recherches
cibËëes apparaissent comme excessËves, voire disproportËonnëes.
Le cadre lëgal fëdëral pertinent ne prëvoit ni le droit, pour les autoritës cantonales, d’accëder ä une
base de donnëes centralisëe ni la crëation ëventuelle de profils de personnalitë. Dës lors, le systëme
SocialPass permet un traitement de donnëes qui va au-delä de ce qui est prëvu par le cadre lëgal
fëdëral
Pour les traitements ëventuellement possibles allant au-delä de ce que prëvoit le cadre lëgal fëdëral,
un motif justificatif au sens de 1’art. 13 al. I'r LPD doit pouvoir ëtre invoquë par les maTtres du fichier
(consentement, intërët prëpondërant privë ou public, base lëgale). Or, dans Ie cas d’espëce, iI semble
que le seul motif justificatif invocable par des maTtres du fichier qui offrent un produit qui permet de
soutenir les ëtablissements accessibles au public dans l’accomplissement d’une täche lëgale en temps
de pandëmie, ne peut qu'ëtre qu’une base lëgale.
La base lëgale entendue comme une norme gënërale et abstraite peut relever du droit cantonal ou
fëdëral. La base lëgale doit ëtre applicable au cas d’espëce et ne pas ëtre contraire ä une autre norme
(hiërarchiquement supërieure).
De plus, le traitement de donnëes justifië sur la base de cette base lëgale doit apparaTtre proportionnë
(cf. WERMELINGER, Stämpflis Handkommentar, Art. 13 DSG N 15).
En l’espëce, le cadre lëgal fëdëral ne prëvoit pas l’accës direct, pour les autoritës cantonales, sur une
base de donnëes centralisëe. En effet, le droit fëdëral applicable au cas d’espëce prëvoit que les
exploitants des ëtablissements accessibles au public maintiennent le contröle sur les coordonnëes
43/62

0
collectëes et ne les transmettent ä l’autoritë publique compëtente uniquement en cas d’infections
prësumëes dans leur ëtablissement.
Toutefois, tant que I'accës direct ä la base de donnëes centralisëe n'entraTne pas un traitement des
donnëes allant au-delä de celui qui serait effectuë si les donnëes ëtaient remises ä I'autoritë sanitaire
sur demande, cet accës semble ëtre justifië, compte tenu de t'intërët public ä lutter contre la pandëmie
actuelle
La question de savoir si et dans quelle mesure les rëglementations cantonales peuventjustifier un accës
plus ëtendu peut ëtre laissëe ouverte sur la base des considërations suivantes :
En effet, le PFPDT peut se prononcer sur la question de savoir si un acte cantonal constitue un motif
justificatif au sens de 1’art, 13 LPD pour un traitement de donnëes effectuë entre personnes privëes.
Dans ce cadre il lui incombe, entre autres, de dëterminer si la base lëgale cantonale est conforme au
droit fëdëral hiërarchiquement supërieur, notamment si le dispositif cantonal est conforme ä la LPD
Ä ce titre, iI convient de distinguer Ia situation dans le canton de Vaud de celle dans le canton du Valais
(cf. lettre du 23 avril 2021 soumise au PFPDT par Lexing Switzerland).
Dans le canton de Vaud, le Chef du Dëpartement de l’ëconomie, de 1’innovation et du sport ainsi que
la Cheffe du Dëpartement de la santë et de l’action sociale vaudois ont ëdictë la Directive du 15
septembre 2020 COVID-19 / Coronavirus. Selon l’art. 4 lit. e de cette Directive, « un dispositif
d’identification de la clientële doit ëtre utilisë systëmatiquement. Ce dispositif doit ëtre homologuë par
la faTtiëre de la branche, en concertation avec I'office du Mëdecin cantonal. Le dispositif d’identification
doit permettre ä garantir la fiabilitë des donnëes collectëes aux fins d’identification des personnes
prësumëes infectëes, en particulier le nom, le prënom et le numëro de tëlëphone mobile. Les donnëes
sont conservëes 14 jours avant destruction. Les donnëes recueillies doivent ëtre rendues accessibles
en tout temps aux autoritës sanitaires dans un format dëfini par ces derniëres >.
Dans Ie document intitulë « Covid-19 – Dispositifs d’identification de la clientële dans les ëtablissements
de restauration – Procëdure de vërification technique – 15 octobre 2020 » (dont l’auteur n’est pas
identifiable), soumis au PFPDT par les reprësentants des parties en annexe au courrier du 23.04.2021,
iI a ëtë prëvu que < les dispositifs d’identËfication doivent rëpondre aux spëcifications techniques
suivantes : [...] – permettre l’enregistrement des donnëes des clients et du personnel sur la base de
donnëes centralisëe gërëe par SwissHelios Särl »
Le mëme document prëvoit, un peu plus bas, qu’« en cas de besoin, l’OMC [office du mëdecin cantonal]
se rend sur la base de donnëes, entre le nom de l’ëtablissement X ä une date et une heure T et peut
extraire un fichier CSV contenant Ia liste des clients et du personnel prësents ä ce moment. Pour
accëder aux donnëes, l’OMC ne doit pas avoir besoin de passer par I'exploitant de l’ëtablissement ou
par les dispositifs d’identification
». S’iI est vrai que la Directive du 15 septembre 2020 est de nature
44/62

0
gënërale et abstraite, force est de constater qu’eIle ne fixe que dans des termes trës gënëraux que les
restaurateurs vaudois doivent utiliser un dispositif d’identification de maniëre systëmatique et que ce
dispositif doit ëtre homologuë par la faTtiëre de la branche, en concertation avec l’office du Mëdecin
cantonal.
Pour Ie reste, et notamment pour la question de savoir si les donnëes collectëes doivent ëtre
enregistrëes sur une base de donnëes centralisëe accessible directement par les autoritës publiques,
cette disposition prëvoit que les autoritës sanitaires sont libres dans le choix des traitements de donnëes
mis en place. Ainsi, l’enregistrement dans une base de donnëes centraËisëe ainsi que le droit d’accës
direct octroyë aux autoritës sanitaires a ëtë prëvu dans Ie document « Covid-19 – Dispositifs
d’identification de la clientële dans les ëtablissements de restauration – Procëdure de vërification
technique – 15 octobre 2020 >.
Cet extrait de document, dont Ia nature juridique reste peu claire, ne constitue clairement pas la nature
d’une norme gënërale et abstraite qui pourrait justifier l’accës dëpassant le cadre de la lëgislation
fëdërale pertinente des autoritës sanitaires. Le PFPDT ne saurait donc admettre que l’accës direct sur
la base de donnëes centralisëe permettant des recherches ciblëes presque indëfinies octroyë au
Mëdecin cantonal vaudois se fonde sur une base lëgale au sens de I'art. 13 al. 1 '' LPD.
En ce qui concerne un ëventuel intërët public prëpondërant comme motifjustificatif au sens de I'art. 13
LPD, iI convient de relever que la lutte contre la pandëmie est une täche publique et non une täche qui
incombe aux personnes privëes, pour quelque raison que ce soit, eIle est rëgie par le droit public. Le
fait que la base lëgale pertinente du Conseil fëdëral ne prëvoit pas d'accës direct doit ëgalement ëtre
considërë comme une indication que des droits d’accës aussi ëtendus n'ont pas ëtë jugës nëcessaires
pour lutter contre la pandëmie, et montre qu’iI s'agit d'un traitement de donnëes inutile et donc
disproportionnë.
Dans le canton du Valais, l’usage du systëme SocialPass a ëtë rendu obligatoire par Dëcision du
Conseil d'Etat du 2 dëcembre 2020 qui se lit comme suit : < la mise en euvre
de 1’application
ëlectronique de tragage SocialPass est obligatoire (ä dëfaut une liste exhaustive de tous les clients >.
Par ailleurs, les dëtails de la mise ä disposition du systëme SocialPass en Valais ont ëtë dëfinis dans le
cadre d’une convention passëe entre I'Etat du Valais, reprësentë par Ie Chef de son Service de la santë
publique, et la sociëtë NewCom4U Särl, ä la fin de l’annëe 2020. L’art. 2.1. dudit contrat oblige la sociëtë
NewCom4U Särl ä fournir une < base de donnëes pour le tra9age via scan ou autoscan de 1’ID
SocialPass ». Dans ce cadre, les SocialPass scannës dans les ëtablissements sont stockës dans la
base de donnëes gërëe par le mandataire et hëbergës dans les serveurs Microsoft Azure localisës dans
Ie canton de Zurich >. La mëme disposition contractuelle prëvoit, un peu plus bas, que < [1]e mandataire
dëveloppe, d'entente et sur la base d'un cahier des charges de 1’Office du mëdecin cantonal, et supporte
la base de donnëes consultable par le Mëdecin cantonal et ses collaborateurs ; le mandataire assure ä
45/62

0
cet effet Ie respect des exigences du Service cantonal de I'informatique pour permettre la consultation
des donnëes par le Mëdecin cantonal et ses collaborateurs depuis le rëseau informatique de
1’administration cantonale ».
La convention conclue entre la sociëtë NewCom4U Särl et 1’Etat du Valais, reprësentë par Ie Chef de
son Service de la santë publique, ne constitue pas une norme gënërale et abstraite pouvantjustifier un
traitement de donnëes au sens de 1’art. 13 al. ler LPD. Dans ce cadre ëgalement, iI n'existe donc pas
de base juridique suffisante qui pourrait justifier un droit d’accës aussi ëtendu octroyë aux autoritës
sanitaires
11 dëcoule de ce qui prëcëde que l’accës direct sur la base de donnëes centralisëe sous sa forme actuelle
(prëvoyant des possibilitës de recherches ciblëes), octroyë aux autoritës cantonales, dëpasse le
traitement de donnëes tel que prëvu et justifië par le droit fëdëral actuellement en vigueur et qu'il n’est
pas justifië par une base lëgale cantonale au sens de I'art. 13 al. 1 " LPD (norme gënërale et abstraite)
et s'avëre comme disproportionnë.
Les responsables de SocialPass doivent donc limiter I'accës des autoritës sanitaires susmentionnëes
aux donnëes nëcessaires pour une collecte lëgale des coordonnëes.
(2) Recommandations
La possibilitë d'accës direct ä la base de donnëes centrale doit ëtre limitëe ä
ce qui est strictement nëcessaire ä la collecte lëgale des coordonnëes, de sorte
qu'eIËe soËt proportionnëe ; en particulier, la possibiËitë de rechercher des
personnes doit ëtre ëliminëe de cette manËëre
Suite ä I'ëlaboration puis ä la notification du rapport et des recommandations dans leur version du 28
mai 2021, deux modifications du cadre lëgal tel que dëcrit au chapitre 3.2.2 doivent ëtre relevëes. Ces
modifications mettent en ëvidence I'absence de base lëgale justifiant les possibilitës de recherches
ciblëes teIles que contestëes dans la recommandation (2) de sorte qu'aucune modification de cette
recommandation n'est indiquëe.
D'une part, iI convient de noter que lors de la visioconfërence du 7juin 2021, le PFPDT a ëtë informë
que la Directive du 15 septembre 2020 COVID-19 /Coronavirus du Chef du Dëpartement de l’ëconomie,
de 1’innovation
et du sport ainsi que de la Cheffe du Dëpartement de la santë et de 1’action sociale
vaudois a ëtë abrogëe en janvier 2021 bien que les reprësentants lëgaux de SocialPass aientjustifië le
traitement
en invoquant cette base lëgale dans leur courrier du 23 avril 2021. Dës lors, les
dëveloppements juridiques figurant au chapitre 3.2.2 du prësent rapport ne sont plus pertinents. En
d’autres termes, dans le canton de Vaud, le traitement de donnëes tel que prëvu par le systëme
SocialPass n’est plus qu’encadrë par le droit fëdëral. Ainsi, en ce qui concerne un ëventuel intërët public
46/62

0
prëpondërant comme motifjustificatif au sens de I'art. 13 LPD, iI convient de rëitërer que la lutte contre
la pandëmie est une täche publique et non une täche qui incombe aux personnes privëes. Pourquelque
raison que ce soit, cette täche est rëgie par le droit public. Dans les cantons oü une disposition cantonale
fait dëfaut, cette täche est exclusivement rëgie par le droit public fëdëral. La base lëgale pertinente du
Conseil fëdëral ne prëvoit pas d'accës direct ä une base de donnëes centralisëe. Les droits d'accës
aussi ëtendus que ceux prëvus par le systëme SocialPass n'ont donc pas ëtë jugës nëcessaires pour
lutter contre la pandëmie et ne sont dës lors par justifËës sur la seule base lëgale pertinente dans le
canton de Vaud.
D'autre part, l’Ordonnance du Conseil fëdëral Covid-19 situation particuliëre, qui encadre la collecte des
coordonnëes dans les ëtablissements accessibles au public a fait I'objet d'une rëvËsion totale de sorte
que la structure et la numërotation des articles ont changë.6 L'art. 11 de l’Ordonnance (auparavant l’art.
5) est dësormais Ia disposition essentielle pour la collecte des donnëes des visiteurs. En sus des
changements formels, I'obligation de collecter les coordonnëes des visiteurs a ëtë rëduite : dans les
restaurants, les clients doivent uniquement partager Ëeurs coordonnëes s'ils prennent place ä I'intërieur.
De plus, une seule personne par groupe doit communiquer ses coordonnëes ä l’exploitant de
l’ëtablissement. Dans les discothëques, l’obligation de collecter les coordonnëes des clients a ëtë
supprimëe. L’accës ä ces ëvënements est toutefois rëservë aux personnes en possession d’un certificat
Covid-19 (Art. 13 Ordonnance COVID-19 situation particuliëre). Dans les centres de sports et lors
d’ëvënements culturels, les coordonnëes doivent toujours ëtre coIËectëes. Les changements
susmentionnës sont entrës en vigueur Ie 26 juin 2021.
3.3.
Option < saisie manuelle »
Le PFPDT constate que, d'une part, les coordonnëes des clients rëguliers sont enregistrëes localement
surl'appareil et que, d'autre part, iI est possible d'exporter ces donnëes vers d'autres appareils au moyen
d'un code QR. En outre, toutes les coordonnëes des clients rëguliers sont affichëes sur les appareils
utilisës par les ëtablissements.
Avec la procëdure choisie, la mise en muvre de I'art. 5 LPD (exactitude des donnëes) requiert un effort
organËsationnel considërable et ne permet mëme pas d’exclure certaines erreurs. Ainsi, les demandes
d'information, de rectification ou d’effacement ne peuvent ëtre traitëes que de maniëre incomplëte.
En outre, I'affichage de toutes les donnëes de contact viole le principe de proportionnalitë tel que
consacrë ä I'art. 4 al. 2 LPD (d’un point de vue temporel et quantitatif), car l’ëtablissement peut consulter
6 Communiquë du Conseil fëdëral du 23.06.2021 https://www.bag.admin,ch/bag/fr/home/das-
bag/aktuell/medienmitteËlungen.msg-id-84127.html,
47/62

0
ä tout moment d’avantage de donnëes sur une personne que ce qui est nëcessaire pour identifier le
client
(3) Recommandation concernant Ia liste des clients rëguliers SocialScan
SocialPass adapte les processus et les fonctions de collecte et de mise ä
disposition des coordonnëes des personnes recourant plusieurs fois ä
I'application (par ex. les clients rëguliers) de sorte que
la collecte des coordonnëes ne soit pas effectuëe par le personnel de service
les coordonnëes des clients rëguliers que l’ëtablissement a enregistrëes
puissent ëtre effacëes ou rectifiëes ä la demande de ces clients
la synchronisation de la liste des clients rëguliers permette d'ëviter des statuts
de donnëes diffërents au sein de la mëme structure, et que les donnëes soient
soumËses ä un cycle de vie axë sur la finalitë
seules les coordonnëes nëcessaires ä l'identification de la liste des clients
rëguliers puissent ëtre consultëes (principe de minimisation des donnëes)
3.4.
Transferts des numëros de tëlëphone aux Ëtats-Unis
Comme indiquë ci-dessus (ch. 2.5.2), les numëros de tëlëphone mobile des utilisateurs sont transmis
au Service Twilio, et donc aux Ëtats-Unis d'Amërique dans le cadre du processus de vërification
Les Ëtats-Unis tombe dans la catëgorie des pays tiers ne disposant pas d’une lëgislation adëquate au
sens de I'art. 6 al. ler LPD7. En dëpit de l’absence d'une lëgislation assurant un niveau de protection
adëquat ä l’ëtranger, I'art. 6 al. 2 LPD prëvoit que des donnëes personnelles peuvent ëtre
communiquëes ä l’ëtranger, ä l’une des conditions prëvues par cet alinëa. En l’espëce, aucune condition
fixëe ä 1’art. 6 al. 2 LPD n’est remplie. Le PFPDT relëve avant tout que des garanties suffisantes,
notamment de nature contractuelle, font dëfaut. II dëcoule de ce qui prëcëde qu’un niveau de protection
adëquat n’a pas ëtë assurë par les responsables.
Mëme si I'intërët (public) invoquë par les responsables afin de justifier la vërification des numëros
semble comprëhensible dans le contexte actuel, force est de constater qu’iI n’est pas apparent pour
quelles raisons il serait nëcessaire de recourir ä un service situë aux Ëtats-Unis, au lieu de mandater
un service similaire ayant son siëge dans un pays offrant un niveau de protection des donnëes adëquat
Par ailleurs, le PFPDT relëve que les personnes concernëes ne sont pas informëes du transfert de leur
numëro de tëlëphone aux Ëtats-Unis, ni mëme de I'utilisation du service Twilio. Aucune information ä
7 Liste des Etats ayant une lëgislation assurant un niveau de protection adëquat, pubIËë sous
https://www.edoeb.admin.ch/dam/edoeb/fr/dokumente/2020/staatenliste.pdf.download.pdf/20200908 Staatenliste f.pdf
48/62

0
propos de Twilio n’est disponible ni sur Ie site internet ni dans les App-Store. Ce manque d’information
constitue une violation du principe de transparence (art. 4 al. 4 LPD).
(4) Recommandation concernant Ie service de vërification des numëros
SocialPass apporte des garanties manifestes (p.ex. au moyen d'un accord
avec Twilio) pour qu’un niveau de protection adëquat soit garanti dans le cadre
du transfert des numëros de tëlëphone des utiËËsateurs au service < Twilio »
aux Etats-Unis ;
Alternativement, SocialPass recourt ä un service alternatif qui n'impËique pas
un transfert vers un pays ëtranger dont Ie niveau de protection est inadëquat.
Les utilisateurs sont informës de maniëre transparente sur Ie transfeR des
donnëes au service de tiers (Twilio ou autre), des modalitës d’enregistrement
et des possibilitës de demander l’effacement des propres donnëes
3.5.
Stockage centralisë et permanent du numëro de tëlëphone mobile dans le processus
d'enregistrement
Le PFPDT note que, pour que le tra9age des contacts fonctionne, iI est entre autres nëcessaire que le
numëro de tëlëphone mobile soit saisi dans SocialPass. Les numëros sont vërifËës au moyen du service
OTP amëricain Twilio (cf. chapitre 2.5.2).
Les numëros de tëlëphone sont ëgalement enregistrës de maniëre centralisëe dans Ia base de donnëe
Azure. Rien n’a ëtë prëvu quant ä leur effacement. Les utilisateurs ne sont pas informës de maniëre
transparente ni de l’enregistrement ni de I'utilisation que Twilio fait de leur numëro. De tels traitements
de donnëes ne rëpondent pas aux exigences fixëes dans la LPD, notamment
au principe de
transparence tel que consacrë ä I'art. 4 al. 4 LPD. En outre, sur la base de I'art. 4 al. 2 LPD, le stockage
centralisë du numëro de tëlëphone mobile lors du processus d’enregistrement est disproportionnë (du
point de vue temporel) dans la mesure oLI ce numëro est conservë pour une durëe illimitëe, c'est-ä-dire
une durëe allant au-delä de ce qui est nëcessaire pour la lutte contre le COVID-19.
centralisë
l’enregistrement
(5) Recommandation
concernant
et
permanent du numëro de tëlëphone mobile dans le processus
d'enregistrement
SocialPass adapte le processus d'inscription des utilisateurs de sorte que
- l’enregistrement centralisë du numëro de tëlëphone mobile soit limitë au strict
nëcessaire pour le traitement visë, notamment en ce qui concerne la durëe de
l’enregistrement (au plus tard lorsque Ia situation particuIËëre prend fin) ;
les utilisateurs, avant d’installer l’application, soient informës de maniëre
transparente quant au traitement de leur numëro de tëlëphone mobile
49/62

0
les utilisateurs soient informës de leurs droits et, en particulier, de la maniëre
dont elles peuvent exercer leurs droits pour que les donnëes en lien avec
I'enregistrement du numëro de tëlëphone mobile soient effacëes
3.6.
Microsoft Azure (base de donnëes SQL)
Deux des trois composants (SocialPass et SocialScan) ont fait I'objet d’une ëvaluation externe de la
sëcuritë. Le troisiëme composant (base de donnëes centrale sur Azure) n'a pas ëtë auditë au motif que
Microsoft est responsable de la sëcuritë. Le PFPDT relëve toutefois qu’en raison de plusieurs risques
liës ä la sëcuritë des donnëes, comme p.ex. la possibilitë d’un data breach, les responsables devraient
ëtre en mesure d’expliquer plus en dëtails pourquoi ils ont renoncë ä un audit adëquat.L’application
SocialPass communique avec une infrastructure centrale (backend) hëbergëe chez Microsoft Azure.
Avec Azure, beaucoup de rëglages sont prëdëfinis, mais d'autres doivent ëtre ajustës manuellement,
comme les alertes et les accës utilisateurs. Pour la sëcuritë de la base de donnëes Azure SQL, iI est
recommandë d’utiliser Azure Sentinel. Cela permet de recueillir des donnëes sur I'ensemble des
utilisateurs,
des appareils, des applications
et des infrastructures
et de dëtecter et d'analyser les
rrienaces .
Azure Sentinel ne permet toutefois pas de configurer, par exemple, des autorisations d’accës pour une
base de donnëes SQL. Or, conformëment
ä I'art. 7 LPD, une teIle configuration est obligatoire du point
de vue de la sëcuritë des donnëes. SocialPass n'a pas encore confirmë au PFPDT que la configuration
dans Azure est mise en auvre conformëment au WhitePaper et ä la Baseline8 applicables (voir ci-
dessous). Le PFPDT constate donc que les recommandations faites par Microsoft (Azure security
baseline) sur la protection de la base de donnëes SQL dans Azure sont insuffisamment mises en @uvre
par SocialPass
(6) Recommandation concernant la configuration et le renforcement de
Microsoft Azure
SocialPass configure la plateforme Microsoft Azure de sorte que
a) les mesures de sëcuritë de la Baseline et du WhitePaper [1] de Microsoft
soient mises en @uvre
b) la vërification de I'efficacitë et la mise en @uvre de ces mesures puissent
ëtre prouvëes
3.7.
Divers aspects de sëcuritë des donnëes
Les responsabËes ont affirmë que des amëliorations concernant la sëcuritë des donnëes ont ëtë mises
en place, sans toutefois les concrëtiser. Les recommandations suivantes dans Ie domaine de la sëcuritë
8 https://docs.microsoft.com/en-us/security/benchmark/azure/baseIËnes/sql-database-security-baseline
(ëtat au 21.4.2021 )
50/62

0
des donnëes sont donc formulëes sous rëserve que les vulnërabilitës
mises en lumiëre dans
l’ëtablissement des faits du 20 mai 2021 n’ont pas ëtë corrigëes entre-temps.
3.7.1. Gestion desvulnërabilitës
Le PFPDT note que les audits externes ont dëcelë des vulnërabilitës. Celles-ci ont ëtë ëvaluëes du point
de vue de la sëcuritë informatique, mais pas de la sëcuritë des donnëes au sens de I'art. 7 LPD en
relation avec I'art. 8 OLPD. Cet aspect a fait l’objet d’une premiëre ëvaluation, par le PFPDT, dans la
section 2.9.4 Afin de garantir la sëcuritë des donnëes conformëment ä 1’art. 7 LPD, iI faudrait classer
toutes les vulnërabilitës (risques ëlevës comme faibles) de maniëre dëcroissante selon leur dangerositë
du point de vue du droit de la protection des donnëes.
(7) Recommandation concernant la gestion des vulnërabilitës
SocialPass adapte les applications SociaËPass et SocialScan de sorte que
a) les vulnërabilitës relevëes dans les rapports d’audit [A] [B] et [C] soient
ëliminëes en fonction des risques qu'elles reprësentent
b) les vulnërabilitës concernant Ia protection des donnëes, en particulier
soient ëltmËnëes sans dëla
3.7.2. Mise en place d’une authentification forte
Le PFPDT constate que, sur la base des informations fournies, iI n'est pas possible de savoir quels
composants du systëme SocialPass sont sëcurisës par I'authentification
ä deux facteurs et donG
protëgës contre tout accës, modification ou destruction non autorisës, si 1’on se rëfëre ä l’ëtat actuel de
la technique et ä I'art. 7 LPD en relation avec I'art. 8 s. OLPD.
(8) Recommandation concernant la mise en place d’une authentification
forte
SocialPass revoit Ë'accës ä tous ses composants de sorte que ceux-ci, en
fonctËon de l’ëtat actuel de la technique, permettent une authentification
robuste, voire y soient obligatoirement soumËs si la protection des donnëes
l’exige
3.7.3.
Utilisation disproportionnëe d'identifiants
Le PFPDT note que, outre le numëro de tëlëphone, le traitement des donnëes dans le cadre de
SocialPass englobe I'IMEI (International Mobile Equipment Identity, un numëro de sërie unique ä quinze
chiffres pour les appareils) et, dans Ie cas d'Android, ëgalement un UID (Unique ID) du numëro
d'utilisateur provenant de Google Firebase. La saisie des donnëes de contact en vue du tragage vise
toutefois les personnes et non les appareils. Les opërateurs n'ont pas expliquë, et les informations
disponibles n’indiquent pas clairement en quoi I'utilisation de ces identifiants est nëcessaire
51 /62

0
Parconsëquent, iI est inutile, et par ce fait, disproportionnë du point de vue de I'art, 4 al. 2 LPD, d’utiliser
des identifiants spëcifiques aux appareils et aux applications ä cette fin. Les numëros de tëlëphone
peuvent trës bien ëtre vërifiës sans que ces identifiants soient utilisës
traitement
(9) Recommandation
identifiants
Ie
des
concernant
d’appareils
SocialPass renonce au traitement des identifiants qui ne sont pas nëcessaires
ä la lumiëre de la finalitë poursuivie, notamment IMEI, Firebase-ID et Unique
ID provenant de Google Firebase
3. 7.4.
Organisation et docume.ntation relatives ä la sëcuritë des donnëes
Les responsables de SocialPass n’ayant pas soumis de documentation relative ä la sëcuritë des
donnëes, dans le cadre de la prësente procëdure, portant sur les responsabilitës en la matiëre, le
PFPDT part du principe qu’une teIle documentation fait dëfaut.
Le PFPDT constate en outre qu'il n'existe pas de rëglement de traitement au sens de I'art. 11 OLPD
incluant une stratëgie de sëcuritë (notamment celle des donnëes) pour SocialPass et SocialScan. Un
tel rëglement sert ä mettre en @uvre et ä documenter la stratëgie de sëcuritë et dëcrit les mesures
techniques et organisationnelles mises en muvre au sens de I'art. 7 LPD
En vertu de 1’art. 11a al. 5 lit. a LPD, les responsables de la base de donnëes ne sont pas soumis ä
l’obligation de dëcËaration d'un fichier, s’iI est assumë que les donnëes sont traitëes par une personne
privëe en vertu d’une obligation lëgale. Par contre, 1’art. 11 OLPD prëvoit l’obligation d'ëlaborer un
rëglement de traitement pour les fichiers automatisës, y compris pour les maTtres de fichiers dëliës de
l’obligation de dëclaration ä condition que cette exception soit basëe sur la lettre a de 1’art. 11a al. 5
LPD
(10)Recommandation concernant la documentation relative ä la sëcuritë
des donnëes
Les responsables de SocialPass se dotent d'un rëglement de traitement
portant notamment sur la sëcuritë des donnëes et proposant une stratëgie de
sëcuritë documentëe qui
comprenne des mesures organisationneIËes et technËques relatives ä la
sëcuritë des donnëes qui soient en phase avec I'ëtat actuel de la
technique
attribue de maniëre claire et documentëe tes täches qu’eIle prëvoit aux
diffërents acteurs
soit rëguliërement contrölëe quant ä l’efficacitë de sa mise en @uvre
52/62

0
4. Prises de position des parties
4.1.
Remarques prëliminaires relatives au droit d’ëtre entendu
Ni 1’art. 29 LPD ni 1’art. 34 OLPD ne contiennent des rëgles spëcifiques quant aux divers dëlais ä
respecter dans le cadre d’une procëdure d’ëtablissement des faits. La pratique du PFPDT en tant
qu’autoritë fëdërale indëpendante consiste ä garantir un dëlai de rëponse raisonnable aux parties afin
que ces derniëres puissent exercer teur droit d’ëtre entendu. Si le PFPDT est tenu de garantir te droit
d’ëtre entendu aux parties impliquëes dans une procëdure d'ëtablissement des faits, les parties elles-
mëmes ont un devoir de collaboration consacrë ä 1’art. 34 LPD.
Lorsque le PFPDT fixe les diffërents dëlais au cours de la procëdure d’ëtablissement des faits, iI procëde
toujours aussi ä une pesëe des intërëts. D'une part, iI prend en compte le besoin pour les parties d’avoir
Ie temps de prëparer leurs soumissions. D’autre part, iI estime que les parties ont un devoir de collaborer
et qu'il leur appartient de lui transmettre toute information utile au bon dëroulement de la procëdure,
p.ex. lorsque certains ëlëments de faits subissent un changement en cours de procëdure. Enfin, ëtant
donnë qu’une procëdure d’ëtablissement des faits n’est qu’engagëe en cas d'« erreur de systëme »,
c’est-ä-dire lorsqu’un traitement risque de porter atteinte ä la personnalitë d’une multitude de personnes,
l’intërët du public ä ëtre informë Ie plus töt possible de cette erreur de systëme est pris en compte dans
la pesëe des intërëts.
La prësente procëdure porte surune application numërique proposëe par deux entreprises privëes dans
toute Ia Suisse pourlutter contre la pandëmie actuelle. Cette application traite des donnëes personnelles
et affecte tout particuliërement Ia population des cantons de Vaud et Valais, notamment en raison des
exigences des autoritës sanitaires de ces deux cantons. Dans ce contexte, le PFPDT s’est efforcë de
faire aboutir la procëdure d’ëtablissement des faits en temps utile. Toutefois, cette procëdure s'est
avërëe exceptionnellement
longue et compliquëe. Lors de la fixation des dëlais de rëponse et de
I'ëvaluation des nombreuses demandes de prolongation de dëlais reQues (cf. chapitre 1.4), le PFPDT a
donc, entre autres, dü tenir compte du fait que, la deuxiëme vague de la pandëmie s’est calmëe au
dëbut de I'ëtë 2021. Cette ëvolution ëpidëmËologique a eu pour consëquence que les restaurants ont pu
rouvrir ä ce moment-lä. Ainsi, une reprise de l’utiËisation de 1’application SocialPass ëtait imminente. Le
PFPDT a donc estimë que la sensibilisation de la population aux risques du traitement de donnëes ëtait
urgente.
4.2.
Prise de position des parties relative aux faits ëtablis Ie 20 mai 2021
Dans le cadre de la prësente procëdure, notamment au vu de la rëouverture des terrasses des
restaurants Ie 19 avril 2021, le PFPDT a remis des recommandations provisoires aux parties Ie 7 avril
2021. Le 23 avril 2021, les parties ont refusë ces recommandations par courrier de Lexing Switzerland
53/62

0
Par lettre du 20 mai 2021, le PFPDT a ensuite communiquë aux parties les faits tels qu’ëtablis au
chapitre 2 afin qu'elles puissent prendre position. Au vu de la rëouverture de l’intërieur des restaurants
Ie 31 mai 2021, le PFPDT a estimë qu'un dëlai de rëponse d'une semaine ëtait approprië au regard des
circonstances particuliëres de la prësente affaire. Les parties ont dëcidë de laisser expirer le dëlai de
rëponse fixë au 27 mai 2021, notamment aprës que le PFPDT ait rejetë et leur demande de prolongation
de dëlai d'au moins 30 jours et la demande de rëcusation des collaborateurs en charge du dossier
soumise par Lexing Switzerland.
4.3.
Prise de position des parties relative au rapport final et aux recommandations du 28
mai 2021
Par courrier du 28 mai 2021, le PFPDT a informë les parties de la fin de la prësente procëdure
d’ëtablissement des faits, leur a remis le prësent rapport et les recommandations y relative dans leur
version du 28 mai 2021 et les a invitëes ä lui faire savoir dans un dëlai de 30 jours, conformëment ä
I'art. 29 al. 4 PFPDT, si elles acceptaient ou rejetaient les recommandatËons.
Par courrier du 14 juin 2021 au PFPDT, Lexing Switzerland a notifië Ia fin de son mandat dans la
prësente procëdure. Cette fin de mandat a conduit le PFPDT ä accorder une prolongation du dëlai de
30 joursjusqu'au 16 juillet 2021, notamment ä la suite d’une demande des parties dësormais agissant
pour leur propre compte. Aprës que les parties aient rëvoquë la demande de rëcusation du personnel
du PFPDT, deux visioconfërences constructives ont eu lieu entre elles et le PFPDT Ie 7 et Ie 24 juin
2021, auxquelles ont ëgalement participë les autoritës de santë et de protection des donnëes ainsi que
les associations de la gastronomie des cantons de Vaud et Valais. Sur la base des ëchanges qui ont
eu lieu dans le cadre de ces deux visioconfërences, les exploitants de SocËalPass ont soumis, le 9 juillet
2021, une prise de position par rapport aux recommandations ëmises par le PFPDT dans son rapport
notifië Ie 28 mai 2021. Le prësent chapitre traite en dëtail des rëponses re9ues.
4.3. 7.
Recommandation (1) concernant les röles et les responsabilitës
La recommandation (1) formulëe ci-dessus au chapitre 3.1 et reprise ci-dessous est la suivante:
(1) Recommandation röles et responsabilitës
Les sociëtës NewCom4U Särl et SwissHeIËos Särl doivent unËformiser tous les
documents (site web, appstores et app) afin de respecter leurs obligations
lëgales en tant que maitres du fichier au sens de 1’art. 3 lit. i LPD
Les exploitants de SocialPass confËrment avoir donnë suite ä cette recommandation, toutefois sans
apporter de prëcËsions (I'affirmation correspondante est limitëe ä « fait »). En tout ëtat de cause, le
PFPDT prend note que les parties acceptent la recommandation
(1) concernant les röles et les
responsabilitës.
54/62

0
Le PFPDT constate en plus que, notamment dans la dëclaration de confidentialitë publiëe sur Ie site
web de SocialPass, seule l’entreprise NewCom4U Särl est mentionnëe comme maitre du fichier.
Toutefois, cela ne correspond pas ä 1’ apprëciation du PFPDT (cf. chapitre 3.1) selon laquelle les deux
sociëtës doivent ëtre considërëes conjointement comme maTtres du fichier. La responsabilitë commune
doit ëtre rendue transparente, c'est-ä-dire que les deux maTtres du fichier doivent figurer de manËëre
cohërente dans la documentation
La recommandation (1) concernant les röles et responsabilitës n'a donc pas encore ëtë complëtement
mise en @uvre ä I'heure actuelle.
4.3.2.
Recommandation (2) concernant Ia base de donnëes centrale
La recommandation (2) formulëe ci-dessus au chapitre 3.2 et reprise ci-dessous est la suivante
(2) Recommandation
La possibilitë d'accës direct ä la base de donnëes centrale doit ëtre limitëe ä
ce qui est strËctement nëcessaire ä la collecte lëgale des coordonnëes, de sorte
qu'elle soit proportionnëe ; en particulier, la possibilitë de rechercher des
personnes doit ëtre ëliminëe de cette maniër9
Les exploitants de SocialPass confËrment avoir donnë suite ä cette recommandation centrale, toutefois
sans apporter de prëcisions (I'affirmation correspondante est limitëe ä ). En tout ëtat de cause,
Ie PFPDT prend note que les parties acceptent la recommandation (2) concernant l’accës direct ä la
base de donnëes centrale et la possibilitë de rechercher des personnes.
4.3.3.
Recommandation (3) concemant Ia liste des clients rëguliers SocialScan
La recommandation (3) formulëe cË-dessus au chapitre 3.3 et reprise ci-dessous est la suivante :
(3) Recommandation concernant Ia liste des clients rëguliers SocialScan
SocialPass adapte les processus et les fonctions de collecte et de mise ä
disposition des coordonnëes des personnes recourant plusieurs fois ä
1’application (par ex. les clients rëguliers) de sorte que
- la collecte des coordonnëes ne soit pas effectuëe par le personnel de service,
- les coordonnëes des clients rëguliers que l’ëtablissement a enregistrëes
puissent ëtre effacëes ou rectifiëes ä la demande de ces clients,
- la synchronisation de la liste des clients rëguliers permette d’ëviter des statuts
de donnëes diffërents au sein de la mëme structure, et que les donnëes soient
soumises ä un cycle de vie axë sur la finalitë,
seules les coordonnëes nëcessairës ä I'identification de la liste des clients
rëguliers puissent ëtre consultëes (principe de minimisation des donnëes)
55/62

0
Ä propos de cette recommandation, la prise de position des exploitants de SocialPass se lit comme
suit
< Ces informations ne sont disponibles que sur les appareils SOCIALSCAN des restaurants et
pas dans Ia base centrale.
a) Cette recommandation n’est pas praticable dans la perspective d’une personne ägëe qui
veut donner ses informations dans l’application. C’est donc au personnel que revient la täche
de saisir ces informations.
b) Cette n’existe pas pour 1’instant et nous prëvoyions de l’implëmenter dans une prochaine
phase de dëveloppement.
c) Le processus de synchronisation
est basë sur la finalitë car iI permet LIne collecte de
donnëes conforme.
d) Seules les informations minimales sont recueillies actuellement ».
Le PFPDT dëduit de cette rëponse que les exploitants acceptent partiellement les recommandations
(3) concernant Ia liste des clients rëguliers SocialScan. II prend acte des remarques quant ä la
praticabilitë de la mise en @uvre des recommandations et dëcidera de la suite ä donner ä cette rëponse
dans le cadre d'ëventuelles contröles de suivi.
4.3.4.
Recommandation (4) concemant Ie service de vërification des numëros
La recommandation (4) formulëe ci-dessus au chapitre 3.4 et reprise ci-dessous est la suivante :
(4) Recommandation concernant Ie service de vërification des numëros
SocialPass apporte des garanties manifestes (p.ex. au moyen d'un accord
avec Twilio) pour qu’un niveau de protection adëquat soit garanti dans le cadre
du transfert des numëros de tëlëphone des utilisateurs au service « Twilio >
aux Etats-Unis ;
Alternativement, SocialPass recourt ä un service alternatif qui n'implique pas
un transfert vers un pays ëtranger dont Ie niveau de protection est inadëquat.
Les utilisateurs sont informës de maniëre transparente sur le transfert des
donnëes au service de tiers (Twilio ou autre), des modalitës d’enregistrement
et des possibilitës de demander I'effacement des propres donnëes
Ä propos de cette recommandation, les exploitants de SocialPass ont soumis au PFPDT Ia prise de
position suivante :
< Twilio a ëtablie des mesures de protection de donnëes qui ëtaient approuvë par la
Communautë Europëenne. Binding Corporate Rules et https://www.twilio.com/gdpr
Nous considërons que cela suffise comme garantie manifeste du niveau de protection de
donnëes.
56/62

0
Twilio ne dispose seulement d’un numëro de tëlëphone qui n'est pas associë ä un nom. Dont,
personne ne pourrait dire je suis xy veuillez effacer mon numëro tel. Le nom xy n'est pas dans
la base de donnëes, seulement un no. de tel. sans identifiant D
Les exploitants n'expliquent pas dans quelle mesure les mesures prësentëes rëpondent aux exigences
du PFPDT en matiëre de garanties suffisantes au sens de la LPD9. Les exploitants ne se prononcent
pas non plus sur l’aspect de la reconnaissabilitë du traitement.
Le PFPDT dëduit de cette rëponse que les exploitants n'acceptent pas les recommandations (4)
concernant Ie service de vërification des numëros. II dëcidera de la suite ä donner ä cette rëponse dans
Ie cadre d'ëventuelles contröles de suivi.
4.3.5. Recommandation (5) concemant l’enregistrement centralisë et permanent du numëro de
tëlëphone mobile dans le processus d'enregistrement
La recommandation (5) formulëe ci-dessus au chapitre 3.5 et reprise d-dessous est la suivante :
(5) Recommandation
l’enregistrement
concernant
centralisë
et
permanent du numëro de tëlëphone mobile dans le processus
d'enregistrement
SocialPass adapte le processus d'inscription des utilisateurs de sorte que
I'enregËstrement centralisë du numëro de tëlëphone mobile soit limitë au
strict nëcessaire pour le traitement visë, notamment en ce qui concerne la
durëe de l’enregistrement (au plus tard lorsque Ia situation particuliëre
prend fin)
les utilisateurs, avant d’installer I'application, soient informës de maniëre
transparente quant au traitement de leur numëro de tëlëphone mobile
les utilisateurs
soient informës de leurs droits et, en particulier, de la
maniëre dont elles peuvent exercer leurs droits pour que les donnëes en
lien avec l’enregistrement du numëro de tëlëphone mobile soient effacëes
Ä propos de cette recommandation, la prise de position des exploitants de SocialPass se lit comme suit
< L’enregistrement centralisë du numëro de tëlëphone est limitë comme recommandë.
Les
utilisateurs
sont
informës
par
la
publication
https://www.socialpass.ch/mentionsleqales/
>
en
9 Cf. https://www.edoeb.admin.ch/edoeb/fr/home/protection-des-donnees/handel-und-wirtschaft/uebermittlung-ins-ausland,html
57/62

0
Le PFPDT prend note que les parties acceptent la recommandation (5) concernant l’enregistrement
centralisë et permanent du numëro de tëlëphone mobile dans le processus d'enregistrement.
Cependant, le PFPDT constate que la dëclaration de confidentialitë mentionnëe ne porte que sur
I'utilisation des donnëes collectëes pour le trag'age des contacts. Or, la recommandation susmentionnëe
fait rëfërence au stockage du numëro de tëlëphone au cours du processus d'enregistrement.
En raison de ce manque de clartë, le PFPDT estime que cette recommandation n’a pas ëtë suivie de
mesures concrëtes et iI en dëduit que la recommandation n'a pas encore ëtë mise en place
complëtement ä I'heure actuelle.
4.3.6.
Recommandation (6) concemant la configuration et le renforcement de Microsoft Azure
La recommandation (6) formulëe ci-dessus au chapitre 3.6 et reprise ci-dessous est la suivante
(6) Recommandation concernant la configuration et le renforcement de
Microsoft Azure
SocialPass configure la plateforme Microsoft Azure de sorte que
a) les mesures de sëcuritë de la Baseline et du WhitePaper [1] de Microsoft
soient mises en @uvre
b) la vërification de I'efficacitë et la mise en @uvre de ces mesures puissent
ëtre prouvëe9
La rëponse des exploËtants de SocialPass ä cette recommandation se lit comme suit:
« En cours d’implëmentation. Disponible d’ici Ia fin du mois d’aoüt. D
Le PFPDT prend note que les parties acceptent la recommandation (6) concernant la configuration et
Ie renforcement de Microsoft Azure et attend les preuves correspondantes dës que la mËse en cnuvre
de cette recommandation aura eu lieu
4.3.7. Recommandation (7) concernant la gestion desvulnërabilitës
La recommandation (7) formulëe ci-dessus au chapitre 3.7.1 et reprise ci-dessous est la suivante :
(7) Recommandation concernant la gestion des vulnërabilitës
SocialPass adapte les applications SocialPass et SocialScan de sorte que
a) les vulnërabilitës relevëes dans les rapports d'audËt [A] [B] et [C 1 soient
ëliminëes en fonction des risques qu’elles reprësentent,
b) les vulnërabilitës concernant Ia protection des donnëes, en particulier
soient ëliminëes sans dëlai.
58/62

0
Les exploitants de SocialPass confirment avoir donnë suite ä cette recommandation, toutefois sans
apporter de prëcisions (l’affirmation correspondante est limitëe ä < fait »). En tout ëtat de cause, le
PFPDT prend note que les parties acceptent la recommandation (7) concernant la gestion des
vulnërabilitës.
4.3.8. Recommandation (8) concernant la mise en place d’une authentification forte
La recommandation (8) formulëe ci-dessus au chapitre 3.7.2 et reprise ci-dessous est la suivante
(8) Recommandation concernant la mise en place d’une authentification
forte
SocialPass revoit I'accës ä tous ses composants de sorte que ceux-ci, en
fonction de l’ëtat actuel de la technique, permettent une authentification
robuste, voire y soient obËigatoirement soumis si la protection des donnëes
l’exige
Les exploitants de SocialPass confirment avoir donnë suite ä cette recommandation, toutefois sans
apporter de prëcisions (I'affirmation correspondante est IËmitëe ä « fait »). En tout ëtat de cause, le
PFPDT prend note que les parties acceptent la recommandation (8) concernant la mise en place d’une
authentification forte
4.3.9. Recommandation (9) concemant le traitement des identifiants d’appareils
La recommandation (9) formulëe ci-dessus au chapitre 3.7.3 et reprise ci-dessous est la suivante
Ie
traitement
des
identifiants
(9) Recommandation concernant
d’appareils
SocialPass renonce au traitement des identifiants qui ne sont pas nëcessaires
ä la lumiëre de la finalitë poursuivie, notamment IMEI, Firebase-ID et Unique
ID provenant de Google Firebase
La prise de position par rapport ä cette recommandation se lit comme suit:
< Nous utilisons un identifiant qui ne correspond pas ä tMEI ou FIREBASE-ID mais qui est
unique et gënërë par 1’application SocialPass >.
Le PFPDT conclut de cette rëponse que les exploitants de SocialPass acceptent la recommandation
(9) concernant le traitement des identifiants d'appareils.
4.3.10. Recommandation (10) concemant la documentation relative ä la sëcuritë des donnëes
La recommandation (10) formulëe ci-dessus au chapitre 3.7.4 et reprise ci-dessous est la suivante
59/62

0
(10) Recommandation concernant la documentation relative ä la sëcuritë
des donnëes
Les responsables de SocialPass se dotent d’un rëglement de traitement
portant notamment sur la sëcuritë des donnëes et proposant une stratëgie de
sëcuritë documentëe qui
comprenne des mesures organisationneIËes et techniques relatives ä la
sëcuritë des donnëes qui soient en phase avec I'ëtat actuel de la
technique
attribue de maniëre claire et documentëe les täches qu’eIle prëvoit aux
diffërents acteurs
soit rëguliërement contrölëe quant ä l’efficacitë de sa mise en muvre
La prise de position par rapport ä cette recommandation se lit comme suit :
« a) Nous allons nous doter d’un organigramme avec des fonctions dëdiëes ä la sëcuritë des
donnëes. 11 sera constituë d’un organe de direction qui veillera ä 1’application des normes en
vigueur concernant Ia protection des donnëes.
b) Nous allons dëlëguer les täches de documentation des processus et de l’exëcution de ces
processus auprës d’une compagnie externe.
c) Nous allons nous doter d’un organe de vërification de l’exëcution et de la maintenance des
processus dëcrit au point b >
Le PFPDT
conclut de cette rëponse que
les exploitants de SocialPass
acceptent
cette
recommandation.
II attend les preuves correspondantes
dës que la mise en muvre de cette
recommandation aura eu IËeu.
5. Conclusion
Depuis le dëbut de la procëdure d'ëtablissement des faits, qui s'est avërëe exceptionnellement longue
et compliquëe, des ajustements importants ont ëtë effectuës par les responsables de SocialPass. En
particulier, les exploitants de SocialPass ont affirmë avoir mis en muvre la recommandation (2)
concernant I'accës direct ä la base de donnëes centrale. Dës lors, le PFPDT suppose que les utilisateurs
de SocialPass ne sont plus exposës ä un accës potentiellement excessif sur leurs coordonnëes de la
part des autoritës sanitaires (via une recherche ciblëe des personnes dans Ia base de donnëes
centrale). De plus, les exploitants ont confirmë au PFPDT que les faiblesses techniques – en particulier
celles relevëes dans les recommandations (6) ä (10) – ont ëtë corrigëes. Les risques d’une atteinte au
droit de la personnalitë des personnes concernëes liës ä I'utilisation de I'application SocialPass ont donc
t,onsidërablement ëtë rëduits au cours de la procëdure. Dans le cadre d’un ëventuel suivi du contröle,
60/62

0
Ie PFPDT reviendra sur les diverses implëmentations des recommandations prëvues et de maniëre
ponctuelle sur d’autres aspects mentionnës dans le prësent rapport.
Au vu de la sensibilitë des donnëes personnelles traitëes et des rëactions de la sociëtë civile, le contröle
du systëme SocialPass quant au respect des exigences de protection des donnëes s'est avërë
nëcessaire et efficace. Les constatations faites et recommandations ëmises par le PFPDT pourront
servir de marche ä suivre pour d’autres exploitants privës, qui souhaiteraient dëvelopper des systëmes
de gestion de rëservations dans le cadre de la lutte contre la pandëmie du Covid-19.
6. Suite de la procëdure
La maniëre dont ces recommandations sont mises en @uvre en pratique relëve de la seule
responsabilitë des exploitants de SocialPass qui sont affligës sur leurs dëclarations et affirmations (art.
34 LPD). Dans le cadre de la poursuite de la coopëration entre les exploitants de SocialPass et le
PFPDT, notamment dans le cadre d'ëventuels contröles ultërieurs, le PFPDT se rëserve le droit de
contröler Ie respect du cadre lëgal par les exploitants de SocialPass.
Dans la mesure oü tesdites sociëtës refusent ou ne suivent pas les recommandations, le PFPDT peut
porter 1’affaire devant Ie Tribunal administratif fëdëral pour dëcision (art. 29 al. 4 LPD)
7. Publication de la recommandation en vertu de 1’art. 30 al. 2 LPD
Pour les raisons susmentionnëes, iI existe un intërët fondamental ä sensibiliser Ie public en temps utile
par rapport aux risques potentiels pour la sphëre privëe et le droit ä I'autodëtermination, qui ëmanent
des applications numëriques dëveloppëes pour lutter contre la pandëmie actuelle. Vu que la procëdure
d’ëtablissement des faits s’est avërëe exceptionnellement longue et compIËquëe, le 31 mai 2021 –jour
de la rëouverture des terrasses des restaurants – le PFPDT a donc informë Ie public quant aux aspects
principaux de la procëdure d’ëtablissement des faits clöturëe Ie 28 mai 2021, y compris par rapport aux
recommandations principales : SocialPass: limitation des possibilitës de recherche requise (admin.ch).
La publication du rapport intëgral dans sa version du 4 aoüt 2021 n’aura lieu que sous rëserve que du
point de vue des sociëtës SwissHelios Särl et NewCom4U Särl aucune donnëe confidentielle qui
pourrait rëvëler des secrets d’affaire ou influencer la capacitë concurrentielle ne figure dans le rapport,
61 /62

0
Les sociëtës SwissHelios Särl et NewCom4U Särl sont priëes de vërifier que le rapport de contröle ne
contienne pas de teIles informations confidentielles et de confirmer cet ëtat de fait par ëcrit au PFPDT
dans un dëlai de 10 jours.
Le Prëposë fëdëral ä la protection
des donnëes et ä la transparence
-.\ .
Lobsiger
Berne, le 4 aoüt 2021
Adrian
62/62
