---
title: "Les smartphones \U0001f4f1"
date: 2022-08-07
---

![android](/smartphones/android.jpg)

Les smartphones sont des éponges à données, ils ont accès à beaucoup d'informations qu'on aimerait garder privées.

Cependant les smartphones (IOS et Android) sont bien plus sécurisés que les systèmes d'exploitation de bureau (Windows, Linux, macOS).
Vous avez remarqué par exemple qu'il y a un système de permission sur les smartphones qu'il n'y a pas sur les PC. Vous savez, les fenêtres qui s'affichent "Autoriser l'accès la position" ou "Autoriser l'accès à la caméra".

Pour les smartphones, les recommandations vont être simples, car je vous recommande uniquement un iPhone ou un Google Pixel.

N'achetez **PAS** de Google Pixel chez votre fournisseur d'accès à Internet (Orange, Free, SFR, Bouygues). Le téléphone est bloqué et vous ne pouvez pas déverrouiller le bootloader comme expliqué plus loin dans [le chapitre dédié](#bootloader). Achetez **toujours** votre téléphone dans les magasins comme la Fnac, Boulanger, Amazon, etc.

Alors oui, je vous voir venir, mais si je vous recommande uniquement ces deux smartphones, c'est parce qu'ils sont les plus sécurisés du marché. Par exemple, vous pouvez mettre un code PIN à 6 chiffres sur ces téléphones (iPhone et Google Pixel), que ça prendrait des dizaines d'années à cracker (normalement, ça prend beaucoup moins de temps sur d'autres marques de téléphones).

Les Google Pixel, à partir du 6, ont [**5 ans de support**](https://support.google.com/pixelphone/answer/4457705?hl=fr#zippy=%2Ct%C3%A9l%C3%A9phones-pixel-et-versions-ult%C3%A9rieures) minimum.

Je vous épargne les détails techniques, mais pour faire très simple, les Google Pixel ne sont pas juste "un peu mieux sécurisés" que les autres marques, ils sont ***excellents en terme de sécurité.***
Je vous conseille donc très fortement de ne rester qu'avec un Google Pixel.

## Le problème de confiance

Il faut comprendre également que sur tous les smartphones Android qui contiennent les applications Google, vous avez une application appelée "`Services Google Play`". Cette application permet de faire beaucoup de choses, cependant, elle a accès à toutes les permissions du téléphone, même les plus sensibles, et sont irrévocables. C'est à cause de cette application que les problèmes de vie privée apparaissent. Android en lui-même n'est pas un problème, c'est l'ajout des applications de Google, et notamment des "`Services Google Play`" qui fait d'Android un cauchemar pour votre vie privée.

Si vous achetez un Samsung par exemple, cela veut dire que vous faites confiance à Google (à cause des `Services Google Play`) **ET** à Samsung pour vos données. Il est donc logique de réduire cette confiance à une seule entité et donc de prendre un Google Pixel.

## Sécurité


### AOSP et firmware

Je vous conseille de prendre un smartphone neuf, c'est à dire encore supporté par le constructeur, voici pourquoi : 

Deux types de mises à jour sont à faire sur un matériel informatique :

- la partie **logicielle**
- la partie **firmware**

La partie **logicielle** est le **système d'exploitation**, donc Android. Mais cela s'applique également à IOS et aux PC avec Windows, MacOS, Linux, ChromeOS, etc. La partie **firmware**, également appelée micrologicielle en français, est une sorte de mini-système d'exploitation pour les composants du matériel (la carte mère, la carte réseau, etc.). Ce n'est pas comme un pilote pour ceux ou celles qui se poseraient la question. 

Je vais rapidement vous expliquer Android pour que vous compreniez bien. Voici un schéma qui vous explique le projet **AOSP** :

![AOSP schéma](/smartphones/aosp.png#center)

**AOSP** signifie **Android Open Source Project**, c'est le cœur de tous les téléphones Android aujourd'hui, AOSP à lui tout seul est très limité : vous n'avez pas d'applications Google par exemple. Comme ce projet est open source (mais détenu par Google) beaucoup de marques (toutes celles qui ne sont pas Apple, donc Samsung, Xiaomi, Huawei, OnePlus, Pocco, et j'en passe) vont prendre le code d'AOSP et le modifier un peu à leur sauce. C'est ce qu'on appelle la **surcouche Android**. **LineageOS** est une surcouche Android développée par des bénévoles.

> ***Quand on parle d'Android, on parle en réalité d'AOSP.***

La surcouche de Samsung par exemple, s'appelle **OneUI**, celle de OnePlus, **OxygenOS**, et celle de Xiaomi s'appelle **MIUI**. Cela fait toujours parti du système d'exploitation, ce ne sont pas des logiciels. Dites-vous qu'AOSP est le moteur d'une voiture avec le chassis, et la surcouche c'est tout le reste.

Cependant, si AOSP est open source, les surcouches ne le sont pas forcément ! LineageOS est une surcouche open source par exemple, mais MIUI ne l'est pas !

> On parle de surcouche, mais en réalité, les constructeurs prennent le projet AOSP pour le modifier selon leurs besoins puis ajouter leurs programmes, leurs fonctionnalités, etc. Ce sont ces modifications et ces ajouts qui sont appellés la surcouche.

Comprenez bien que si vous souhaitez installer LineageOS sur votre téléphone, cela veut dire que vous supprimez le système d'exploitation de votre téléphone. En gros, si vous allumez votre téléphone après avoir supprimé le système d'exploitation de Samsung par exemple, vous ne pourrez plus démarrer votre téléphone, car il n'y aura rien à démarrer ! Sauf si vous installez LineageOS juste après, évidemment 😁.

Si vous changer le système d'exploitation de votre téléphone Android avec un autre Android, imaginons par exemple que vous avez un Samsung et que vous souhaitez installer LineageOS à la place de OneUI, vous pourrez en effet toujours bénéficier des mises à jour d'Android (grâce aux bénévoles de LineageOS) même si Samsung a arrêté le support de votre smartphone. Cependant, le firmware ne pourra jamais être mise à jour, car uniquement Samsung peut le faire ! C'est un énorme risque de sécurité qui ne devrait pas être pris à la légère !

Le firmware, pour expliquer grossièrement, ne fait pas parti du système d'exploitation d'Android. C'est le mini-système d'exploitation des composants intégrés à votre téléphone.

C'est pour cela que je vous recommande un Google Pixel. Je vous conseille même de prendre au minimum un Google Pixel 6 (ou 6 pro, ou 6a), car tous les Google Pixel à partir du 6, bénéficieront de [5 ans de mises à jour de sécurité](https://support.google.com/pixelphone/answer/4457705?hl=fr#zippy=%2Ct%C3%A9l%C3%A9phones-pixel-et-versions-ult%C3%A9rieures) minimum !

---

Cependant, je vous **DÉCONSEILLE** d'installer LineageOS sur votre téléphone, car vous devez déverrouiller le bootloader, et cela détruit tout le modèle de sécurité d'Android. Je vous conseille soit de garder l'Android que vous avez par défaut, ou alors d'installer GrapheneOS, car vous pouvez reverrouiller le bootloader.

---

### Bootloader

Pour faire simple, le [bootloader](https://www.reddit.com/r/LineageOS/comments/n7yo7u/a_discussion_about_bootloader_lockingunlocking/) est la partie qui cherche ce qu'il faut démarrer (ici, Android) juste après la mise sous tension de l'appareil. Le bootloader possède une fonctionnalité appelée " Android Verified Boot" (AVB) ou "démarrage sécurisé" en français. AVB permet entre autre de vérifier que le système d'exploitation est correct et n'a pas été modifié (par un virus, par quelqu'un ou par autre chose) ! Si le système avait été modifié, AVB aurait annulé ces modifications au démarrage !

Si vous déverrouiller votre bootloader, AVB sera désactivé, et donc vous aurez un manque total de sécurité sur votre smartphone.

Vous ne pouvez pas reverrouiller votre smartphone avec LineageOS, mais vous pouvez cependant le faire avec GrapheneOS ! J'écrirai un tuto, très détaillé pour expliquer l'installation de ce dernier, ne vous inquiétez pas, c'est moins compliqué qu'il n'y paraît 😉, et tout fonctionnera pareil que d'habitude (mais en plus sécurisé).

### Antivirus

Pour la sécurité de votre smartphone, [n'installez **PAS**](https://privsec.dev/os/android-tips/#manage-android-permissions) d'antivirus, gratuits ou payants.
Je vous suggère de lire l'article de Wonderfall concernant la [sécurité sur les smartphones](https://wonderfall.space/modele-securite-mobile/).

### Code PIN

Je vous ***déconseille très fortement*** d'utiliser des [schémas](https://wonderfall.space/password/#le-cas-dun-smartphone) (ou [patterns](https://privsec.dev/os/android-tips/#use-a-diceware-passphrase-avoid-pattern-unlock)) pour déverouiller votre téléphone. Une [étude](/smartphones/Cracking-Android-Pattern-Lock-in-Five-Attempts.pdf), a prouvé l'inefficacité des schémas. Si vous posséder un Google Pixel ou un iPhone vous pouvez utiliser un code PIN, ces deux téléphones sont tellement sécurisés que juste mettre un code PIN à 4 chiffres prendrait plusieurs dizaines d'années à être [bruteforce](/basiques/password-managers#pourquoi-un-mot-de-passe-doit-comporter-des-majuscules-et-des-caract%C3%A8res-sp%C3%A9ciaux-) (mais mettez quand même 8 chiffres au minimum).

De manière générale, je vous conseille d'utiliser un code PIN à 6 chiffres. Cependant, il serait plus avisé de mettre un code PIN de 8 chiffres ou plus. Et non ne mettez **pas** la vitesse de la lumière, le nombre pi, ou n'importe quelle autre constante mathématique. Et surtout ne mettez pas votre date de naissance, celle d'un proche ou de votre animal.

Vous pouvez, en complément, utiliser l'empreinte digitale, cela évitera que les gens vous voient taper votre code PIN.

## Le problème des prix

Alors oui la sécurité et la vie privée ont très souvent un prix, je vous conseille donc de prendre la version "a" des Google Pixel, comme le Google Pixel 6a, et de l'acheter après que Google sorte le Pixel 7 vers Octobre 2022, vous aurez peut-être des réductions car Google essayera de vider ses stocks de Google Pixel 6a. De plus, si vous achetez des smartphones à 200€ tels que les Xiaomi par exemple, vous perdrez plus d'argent car un Xiaomi (et croyez-moi par expérience) ne tient jamais long feu (grand maximum 2 ans) et le support s'arrête au bout de 2 ans. Si vous rachetez un smartphone tous les 2 ans, au bout de 5 ans vous aurez payé 500€ (200+200+100). Si vous achetez un Google Pixel 6a au prix fort, 470€ au moment où je vous écris, vous économisez bien 30€, voire plus si vous arrivez à avoir des réductions sur le Google Pixel.

Car en effet je vous conseille de garder votre smartphone jusqu'à ce que :

1. Le support s'arrête
2. Il soit tellement cassé qu'il soit inutilisable

## Fairphone

Je vous déconseille fortement le Fairphone car il n'est pas sécurisé par défaut. En effet, Fairphone met à jour leurs téléphones pendant plusieurs années (leur premier téléphone de 2013 est toujours mise à jour) mais ne met pas à jour les firmwares ! Car seuls les constructeurs Qualcomm peuvent le faire !

Qualcomm est l'entreprise qui créée la plupart des composants tels que les processeurs, puces graphiques, cartes mères pour la plupart des smartphones (Samsung, Xiaomi, OnePlus, Fairphone, etc.).

De plus, Fairphone utilise souvent les avant-derniers processeurs et autres composants de Qualcomm, sachant que Qualcomm met à jour ses composants pendant environ 3 ans, Fairphone utilise donc des composants qui sont en fin de support. Pour réitérer, quand vous achetez un Fairphone, vous achetez un smartphone qui n'est déjà presque plus supporté par les constructeurs !!! C'est un gros problème de sécurité !

Alors évidemment, je suis pour l'écologie et la protection de l'environnement, mais il faut avoir une bonne balance entre sécurité, vie privée et écologie. Si vous prenez un Xiaomi par exemple, vous n'avez ni sécurité (par rapport à un Google Pixel ou un iPhone), ni respect de votre vie privée, ni respect de l'environnement. En prenant un Fairphone, vous respectez un peu l'environnement (ça reste polluant de fabriquer un smartphone), vous n'avez pas de vie privée (les Services Google Play sont toujours là) et pas de sécurité du tout ! Avec un Google Pixel, vous gagnez en sécurité, et en écologie car vous gardez votre téléphone 5 ans, mais vous ne gagnez toujours pas en vie privée. Cependant, si vous installez GrapheneOS sur votre Pixel, vous gagnez en sécurité, écologie et en vie privée !

## Conclusion

Pour réitérer :

- Prenez un Google Pixel (à partir du 6, car 5 ans de support) ou un iPhone récent.
- N'installez pas d'applications qui se disent améliorer la sécurité ou la performance de votre téléphone.
- Utilisez un code PIN de 6 chiffres minimum, mais 8 chiffres ou plus est recommandé.
- Installez GrapheneOS sur votre Google Pixel.
- Achetez uniquement des téléphones neufs ou quasi-neufs. N'achetez pas de téléphones qui ne sont plus supportés.

---

## En savoir plus

- [Le modèle de sécurité mobile - Wonderfall](https://wonderfall.space/modele-securite-mobile/)
- [Android - Madaidan (en anglais)](https://madaidans-insecurities.github.io/android.html)
- [Android Tips - PrivSec.dev (en anglais)](https://privsec.dev/os/android-tips/)*(site en anglais, j'ai le même thème que son site web car c'est un thème publique et gratuit, ne soyez pas étonné)*