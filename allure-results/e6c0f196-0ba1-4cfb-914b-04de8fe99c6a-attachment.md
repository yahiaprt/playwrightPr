# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: profil.spec.ts >> US-03 : Modification du profil entreprise
- Location: tests\profil.spec.ts:4:5

# Error details

```
Test timeout of 30000ms exceeded.
```

```
Error: page.goto: Test timeout of 30000ms exceeded.
Call log:
  - navigating to "https://thrundrz.fr/gestion/", waiting until "load"

```

# Page snapshot

```yaml
- generic [ref=e2]:
  - banner [ref=e3]:
    - navigation [ref=e4]:
      - generic:
        - link "gestion freelance":
          - /url: /
          - img "gestion freelance"
      - list [ref=e6]:
        - listitem [ref=e7] [cursor=pointer]:
          - link "Accueil" [ref=e8]:
            - /url: /
        - listitem [ref=e9] [cursor=pointer]: Accompagner
        - listitem [ref=e10] [cursor=pointer]: Services
        - listitem [ref=e11] [cursor=pointer]: Tarifs
      - generic [ref=e12]:
        - link "Influenceur ?" [ref=e13] [cursor=pointer]:
          - /url: /gestion/influenceur/register
        - link "Se connecter" [ref=e14] [cursor=pointer]:
          - /url: /gestion/login
        - link "Création du compte" [ref=e15] [cursor=pointer]:
          - /url: /gestion/newcompte
  - main [ref=e16]:
    - generic [ref=e17]:
      - generic [ref=e18]:
        - generic [ref=e19]:
          - paragraph [ref=e20]: AUTOMATISEZ VOTRE GESTION
          - paragraph [ref=e21]: Toute votre gestion freelance, réunie en un seul endroit.
        - paragraph [ref=e22]: Créez vos devis et factures en quelques clics et relancez vos clients automatiquement.
        - button "Contactez-Nous" [ref=e23] [cursor=pointer]
      - generic:
        - img "gestion freelance"
    - generic [ref=e24]:
      - generic [ref=e25]:
        - generic [ref=e26]:
          - paragraph [ref=e27]: Organisez tous vos clients facilement
          - paragraph [ref=e28]: Simplifiez la gestion de vos clients en regroupant toutes leurs informations au même endroit. Ajoutez de nouveaux contacts, suivez vos interactions et retrouvez rapidement chaque détail pour optimiser votre temps et améliorer votre relation client.
          - list [ref=e29]:
            - listitem [ref=e30]:
              - img [ref=e31]
              - generic [ref=e33]: Ajouter et gérer vos clients
            - listitem [ref=e34]:
              - img [ref=e35]
              - generic [ref=e37]: Suivre les interactions et échanges
            - listitem [ref=e38]:
              - img [ref=e39]
              - generic [ref=e41]: Retrouver les informations rapidement
        - generic:
          - img "gestion freelance"
      - generic [ref=e42]:
        - generic [ref=e43]:
          - paragraph [ref=e44]: Créez vos devis et factures
          - paragraph [ref=e45]: Créez, modifiez ou supprimez vos devis et factures en quelques clics. Filtrez-les facilement par statut et téléchargez-les instantanément en PDF.
          - list [ref=e46]:
            - listitem [ref=e47]:
              - img [ref=e48]
              - generic [ref=e50]: Créer et modifier des devis
            - listitem [ref=e51]:
              - img [ref=e52]
              - generic [ref=e54]: Générer des factures PDF
            - listitem [ref=e55]:
              - img [ref=e56]
              - generic [ref=e58]: Filtrer par statut
        - generic:
          - img "gestion freelance"
      - generic [ref=e59]:
        - generic [ref=e60]:
          - paragraph [ref=e61]: Automatisez vos relances clients
          - paragraph [ref=e62]: Envoyez vos relances en un seul clic grâce à des messages personnalisés et automatiques. Gagnez du temps et assurez un suivi professionnel de vos paiements.
          - list [ref=e63]:
            - listitem [ref=e64]:
              - img [ref=e65]
              - generic [ref=e67]: Envoyer des relances automatiques
            - listitem [ref=e68]:
              - img [ref=e69]
              - generic [ref=e71]: Personnaliser les messages
            - listitem [ref=e72]:
              - img [ref=e73]
              - generic [ref=e75]: Suivi des paiements en un clic
        - generic:
          - img "gestion freelance"
      - generic [ref=e76]:
        - generic [ref=e77]:
          - paragraph [ref=e78]: Partage facile avec votre comptable
          - paragraph [ref=e79]: Invitez votre comptable en toute simplicité, exportez vos données en CSV et envoyez-les automatiquement par e-mail. Facilitez vos échanges et gagnez un temps précieux.
          - list [ref=e80]:
            - listitem [ref=e81]:
              - img [ref=e82]
              - generic [ref=e84]: Inviter votre comptable
            - listitem [ref=e85]:
              - img [ref=e86]
              - generic [ref=e88]: Exporter les données en CSV
            - listitem [ref=e89]:
              - img [ref=e90]
              - generic [ref=e92]: Envoyer automatiquement par e-mail
        - generic:
          - img "gestion freelance"
    - generic [ref=e93]:
      - heading "Facilitez vos démarches avec notre équipe de gestion" [level=1] [ref=e94]
      - paragraph [ref=e95]: Pour seulement 29,90 €, envoyez-nous votre Kbis et votre pièce d’identité. Notre service de gestion pourra, à votre demande, procéder à votre inscription et établir votre premier devis en fonction des informations fournies.
      - button "Contactez-Nous" [ref=e97] [cursor=pointer]
    - generic [ref=e98]:
      - heading "Abonnements adaptés à vos besoins" [level=2] [ref=e99]
      - generic [ref=e100]:
        - button "Mensuelle" [ref=e101] [cursor=pointer]
        - button "Annuelle (-10%)" [ref=e102] [cursor=pointer]
      - generic [ref=e103]:
        - generic [ref=e104]:
          - generic [ref=e105]:
            - paragraph [ref=e106]: Basic
            - paragraph [ref=e107]: Faites un essai et testez vos super-pouvoirs
            - paragraph [ref=e108]: € / mois
            - paragraph [ref=e109]: "0"
          - generic [ref=e110]:
            - generic [ref=e111]:
              - img [ref=e112]
              - paragraph [ref=e114]: 2 factures/devis par mois
            - generic [ref=e115]:
              - img [ref=e116]
              - paragraph [ref=e118]: 1 client max
            - generic [ref=e119]:
              - img [ref=e120]
              - paragraph [ref=e122]: Relances manuelles seulement
            - generic [ref=e123]:
              - img [ref=e124]
              - paragraph [ref=e126]: Support par email (réponse sous 48h)
          - paragraph [ref=e127] [cursor=pointer]: S'inscrire gratuitement
        - generic [ref=e128]:
          - generic [ref=e129]: Populaire
          - generic [ref=e130]:
            - paragraph [ref=e131]: Pro
            - paragraph [ref=e132]: Expérimentez la puissance
            - paragraph [ref=e133]: € / mois
            - paragraph [ref=e134]: "9.99"
          - generic [ref=e135]:
            - generic [ref=e136]:
              - img [ref=e137]
              - paragraph [ref=e139]: Factures, devis et clients illimités
            - generic [ref=e140]:
              - img [ref=e141]
              - paragraph [ref=e143]: Relances manuelle et automatique
            - generic [ref=e144]:
              - img [ref=e145]
              - paragraph [ref=e147]: Exporter données Exel/CSV
            - generic [ref=e148]:
              - img [ref=e149]
              - paragraph [ref=e151]: Personnalisation PDF
            - generic [ref=e152]:
              - img [ref=e153]
              - paragraph [ref=e155]: Support par email (réponse sous 24h)
          - paragraph [ref=e156] [cursor=pointer]: Passer à Pro
        - generic [ref=e157]:
          - generic [ref=e158]:
            - paragraph [ref=e159]: Business
            - paragraph [ref=e160]: Prenez le contrôle de votre business, concentrez-vous sur l’essentiel
            - paragraph [ref=e161]: € / mois
            - paragraph [ref=e162]: "19.99"
          - generic [ref=e163]:
            - generic [ref=e164]:
              - img [ref=e165]
              - paragraph [ref=e167]: Tout le plan Pro
            - generic [ref=e168]:
              - img [ref=e169]
              - paragraph [ref=e171]: Invitez votre comptable
            - generic [ref=e172]:
              - img [ref=e173]
              - paragraph [ref=e175]: Intégration chat en direct
          - paragraph [ref=e176] [cursor=pointer]: Passer à Business
    - generic [ref=e177]:
      - heading "Gérer vos devis et factures n’a jamais été aussi simple" [level=1] [ref=e178]
      - generic [ref=e179]:
        - generic [ref=e180]:
          - img [ref=e181]
          - paragraph [ref=e183]: Disponible 100 % en ligne
        - generic [ref=e184]:
          - img [ref=e185]
          - paragraph [ref=e187]: Invitation du comptable
        - generic [ref=e188]:
          - img [ref=e189]
          - paragraph [ref=e192]: Relances automatiques
        - generic [ref=e193]:
          - img [ref=e194]
          - paragraph [ref=e196]: Export PDF illimité
    - generic [ref=e197]:
      - heading "Besoin d’aide ? On a les réponses" [level=2] [ref=e198]
      - generic [ref=e199]:
        - generic [ref=e200]:
          - heading "Que faire après ma première connexion ?" [level=3] [ref=e201]
          - paragraph [ref=e202]: "Commencez par compléter votre profil dans la section Profil & Abonnement. Remplissez toutes les informations obligatoires de votre société : nom commercial, statut juridique, logo, SIRET (obligatoire et unique), TVA et email principal (unique). Ces informations sont essentielles pour créer des devis et factures conformes."
        - generic [ref=e203]:
          - heading "Comment ajouter un client ?" [level=3] [ref=e204]
          - paragraph [ref=e205]: Avant de créer un devis ou une facture, ajoutez au moins un client dans la liste des clients. Cliquez sur 'Ajouter un client' et remplissez les informations nécessaires.
        - generic [ref=e206]:
          - heading "Comment créer un devis ?" [level=3] [ref=e207]
          - paragraph [ref=e208]: "Après avoir ajouté un client, rendez-vous dans la section Devis. Chaque devis reçoit un numéro unique (ex : DEV-0001). Vous pouvez transformer le devis en facture via le bouton 'Transformer en facture'."
        - generic [ref=e209]:
          - heading "Comment générer et télécharger un PDF ?" [level=3] [ref=e210]
          - paragraph [ref=e211]: Pour chaque devis ou facture, utilisez le bouton PDF pour télécharger le document. Cela permet de partager facilement vos documents avec vos clients.
        - generic [ref=e212]:
          - heading "Comment personnaliser le PDF ?" [level=3] [ref=e213]
          - paragraph [ref=e214]: Vous pouvez configurer vos PDF en choisissant si vous souhaitez inclure le logo de votre société et la couleur du PDF. Cela permet de créer des documents professionnels et cohérents avec votre identité visuelle.
        - generic [ref=e215]:
          - heading "Comment relancer une facture impayée ?" [level=3] [ref=e216]
          - paragraph [ref=e217]: Dans la liste des factures, cliquez sur 'Relancer' et personnalisez le message avant l'envoi. Les relances suivantes sont automatiques tous les 15 jours tant que le statut de la facture reste non payé.
        - generic [ref=e218]:
          - heading "Quelles informations sont importantes pour la TVA ?" [level=3] [ref=e219]
          - paragraph [ref=e220]: Assurez-vous que le SIRET et le numéro de TVA sont corrects dans votre profil. Ces informations apparaîtront sur tous vos devis et factures officiels.
        - generic [ref=e221]:
          - heading "Puis-je utiliser un téléphone pour gérer mes documents ?" [level=3] [ref=e222]
          - paragraph [ref=e223]: Il est recommandé d’utiliser un ordinateur pour configurer le profil, ajouter des clients et créer des devis/factures afin d’éviter les erreurs et profiter d’une meilleure expérience utilisateur.
    - generic [ref=e224]:
      - generic [ref=e225]:
        - paragraph [ref=e226]: Nous sommes là pour vous
        - paragraph [ref=e227]: Vous avez des questions ? Besoin d'une démonstration ou d’un accompagnement personnalisé ? Remplissez le formulaire et nous organiserons un appel pour vous guider pas à pas.
        - list [ref=e228]:
          - listitem [ref=e229]:
            - img [ref=e230]
            - generic [ref=e232]: Nous sommes disponibles pour répondre à toutes vos questions
          - listitem [ref=e233]:
            - img [ref=e234]
            - generic [ref=e236]: Organiser un appel ou une démonstration
          - listitem [ref=e237]:
            - img [ref=e238]
            - generic [ref=e240]: Vous guider pour vos devis et factures
          - listitem [ref=e241]:
            - img [ref=e242]
            - generic [ref=e244]: Support et suivi personnalisé
      - generic [ref=e246]:
        - generic [ref=e247]:
          - generic [ref=e248]:
            - img [ref=e249]
            - textbox "Société" [ref=e252]
          - generic [ref=e253]:
            - img [ref=e254]
            - textbox "SIRET" [ref=e257]
        - generic [ref=e258]:
          - generic [ref=e259]:
            - img [ref=e260]
            - textbox "Nom" [ref=e262]
          - generic [ref=e263]:
            - img [ref=e264]
            - textbox "Prénom" [ref=e266]
        - generic [ref=e267]:
          - generic [ref=e268]:
            - img [ref=e269]
            - textbox "Email" [ref=e271]
          - generic [ref=e272]:
            - img [ref=e273]
            - textbox "Téléphone" [ref=e275]
        - textbox "Objet du message" [ref=e277]
        - textbox "Message" [ref=e279]
        - button "Envoyer" [ref=e281] [cursor=pointer]
      - region "Notifications Alt+T"
  - contentinfo [ref=e282]:
    - generic [ref=e283]:
      - generic [ref=e284]:
        - generic [ref=e285]:
          - link "gestion freelance":
            - /url: /
            - img "gestion freelance"
          - paragraph [ref=e286]: Notre plateforme a été pensée pour la nouvelle génération de freelances et d’indépendants. Nous créons un espace de gestion plus simple et plus efficace, partout dans le monde.
        - generic [ref=e287]:
          - heading "Raccourcis" [level=4] [ref=e288]
          - generic [ref=e289] [cursor=pointer]: Accueil
          - generic [ref=e290] [cursor=pointer]: Accompagner
          - generic [ref=e291] [cursor=pointer]: Services
          - generic [ref=e292] [cursor=pointer]: Tarifs
        - generic [ref=e293]:
          - heading "Services" [level=4] [ref=e294]
          - paragraph [ref=e295]: Création devis
          - paragraph [ref=e296]: Facture
          - paragraph [ref=e297]: Gérer vos clients
          - paragraph [ref=e298]: Inviter comptable
          - paragraph [ref=e299]: Relancer vos clients
        - generic [ref=e300]:
          - heading "Contactez-nous" [level=4] [ref=e301]
          - paragraph [ref=e302]: contact@gestionfreelance.com
          - paragraph [ref=e303]: Lyon 69000
        - generic [ref=e304]:
          - heading "Suivez-nous" [level=4] [ref=e305]
          - generic [ref=e306]:
            - img [ref=e307] [cursor=pointer]
            - img [ref=e309] [cursor=pointer]
            - img [ref=e311] [cursor=pointer]
      - separator [ref=e313]
      - generic [ref=e314]:
        - generic [ref=e315]:
          - link "Mentions légales" [ref=e316] [cursor=pointer]:
            - /url: /mentions-legales
          - link "Conditions générales de ventes" [ref=e317] [cursor=pointer]:
            - /url: /conditions-ventes
          - link "Politiques de confidentialité" [ref=e318] [cursor=pointer]:
            - /url: /politique-confidentialite
          - link "Politique Cookies" [ref=e319] [cursor=pointer]:
            - /url: /politique-cookies
          - link "Déclaration Accessibilité" [ref=e320] [cursor=pointer]:
            - /url: /declaration-accessibilite
        - paragraph [ref=e321]: Copyright © Gestion Freelance
```

# Test source

```ts
  1  | import {expect, test } from '@playwright/test'
  2  | 
  3  | 
  4  | test("US-03 : Modification du profil entreprise", async function ({page}){
> 5  |     await page.goto("https://thrundrz.fr/gestion/")
     |                ^ Error: page.goto: Test timeout of 30000ms exceeded.
  6  |     
  7  |     // cliquer sur la bouton creer un compt
  8  |     await page.getByRole("link", {name:"Se connecter"}).click()
  9  | 
  10 |     // Email 
  11 |     await page.locator("#email").fill("yahia2248@gmail.com")
  12 |     await page.locator("#password").fill("]DS+C@94!yUhxjd@3")
  13 | 
  14 |     await page.getByRole("button", {name: "Se connecter"}).click()
  15 |     //clique sur profil
  16 |     await page.getByRole("button", {name: "Profil"}).click()
  17 |     // modifier Forme juridique
  18 |     await page.locator("[name = 'forme_juridique']").selectOption("SASU")
  19 |     //cocher les cases 10 et 20
  20 |     await page.getByRole("checkbox", {name: "10%"}).check()
  21 |     await page.getByRole("checkbox", {name: "20%"}).check()
  22 | 
  23 |     //clique sur sauvgarder
  24 |     await page.getByRole("button", {name: "Sauvegarder"}).click()
  25 | 
  26 |     //verifier c été bien modifier
  27 |     await expect(page.locator("[role='alert']",{hasText:"Profil mis à jour avec succès"})).toBeVisible()
  28 |     
  29 | })
```