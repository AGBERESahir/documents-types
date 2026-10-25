# documents-types

Rédige en deux minutes une **lettre de réclamation**, une **attestation sur l'honneur** ou une **demande administrative**, puis enregistre-la en PDF ou imprime-la.

**Démo : https://agberesahir.github.io/documents-types/**

- Un seul fichier HTML, aucune installation, aucun compte.
- **Rien n'est envoyé ni enregistré** : le texte se construit dans ton navigateur et disparaît quand tu fermes la page.
- Mode sombre pour l'écran, mise en page papier propre à l'impression.

## Les trois modèles

| Modèle | Pour quoi faire | Champ « objet » | Délai de réponse |
|---|---|---|---|
| Lettre de réclamation | Contester une facture, un service non rendu, un retard | *Objet de la réclamation* | Oui (15 jours par défaut) |
| Attestation sur l'honneur | Déclarer sur l'honneur un fait (hébergement, situation, etc.) | *Ce que tu atteste* | Non |
| Demande administrative | Demander un document, un rendez-vous, un remboursement | *Ce que tu demandes* | Oui (15 jours par défaut) |

Chaque lettre contient automatiquement l'expéditeur, le destinataire, le lieu et la date du jour, l'objet, la formule de politesse et la signature. Les champs vides sont remplacés par des repères entre crochets (`[Ton nom]`, `[Ville]`, `[Destinataire]`) pour que tu voies ce qu'il reste à compléter.

## Comment l'utiliser

1. Choisis le **type de document**.
2. Remplis ton nom, ta ville, l'objet et, si besoin, ton adresse, le destinataire et les détails (faits, dates, montants).
3. L'aperçu de la lettre se met à jour à chaque frappe.
4. Clique sur **Imprimer ou enregistrer en PDF**, puis choisis « Enregistrer au format PDF » comme imprimante. Seule la lettre est imprimée, sans le formulaire.
5. Ou clique sur **Copier le texte** pour le coller dans un e-mail ou un traitement de texte.

### Exemple de rendu (demande administrative)

```text
Awa Koffi
12 rue des Manguiers
                                              Mairie de Lomé, service de l'état civil
                                                          Lomé, le 25 octobre 2026

Objet : demande de la copie intégrale de mon acte de naissance

Madame, Monsieur,

Je me permets de solliciter la copie intégrale de mon acte de naissance.

Je reste à votre disposition pour tout justificatif complémentaire et vous remercie
de bien vouloir me répondre sous 15 jours.

Je vous prie d'agréer, Madame, Monsieur, l'expression de mes salutations distinguées.
                                                                           Awa Koffi
```

Dans cet exemple, le champ « Ce que tu demandes » contient `la copie intégrale de mon acte de naissance`.

**Astuce de rédaction** : le même texte est repris dans l'objet (« demande de … ») et dans la phrase d'ouverture (« Je me permets de solliciter … »). Écris-le donc sous une forme qui se lit bien dans les deux, avec son article (« la copie… », « un rendez-vous… »). L'exemple ci-dessus est une illustration de la structure : la page applique l'alignement à droite du destinataire et de la date.

## Limites

- **Ce sont des points de départ, pas un avis juridique.** Adapte le texte à ta situation. Pour un litige important, fais relire la lettre.
- Les modèles sont écrits en **français** et suivent les usages d'un courrier formel. Les formules de politesse sont figées.
- La phrase de la réclamation « je me réserve le droit de saisir les organismes compétents » est générique : retire-la ou précise-la selon ton cas.
- **Rien n'est sauvegardé.** Si tu recharges la page, les champs sont vides. Copie ou exporte avant de fermer.
- Pas de pièces jointes, de signature manuscrite ni de numéro de recommandé : ajoute-les toi-même.
- Garde une **copie datée** de chaque courrier envoyé, et préfère un envoi avec accusé de réception pour une réclamation.

## Utiliser en local

```bash
git clone https://github.com/AGBERESahir/documents-types.git
cd documents-types
# puis ouvre index.html dans ton navigateur
```

Seule la police Atkinson Hyperlegible est chargée depuis Google Fonts ; sans connexion, la police système la remplace.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Formulaire, génération des lettres, impression. |
| `shared.css` | Styles communs avec [frais-transfert](https://github.com/AGBERESahir/frais-transfert) et [rappels-echeances](https://github.com/AGBERESahir/rappels-echeances). |

## Licence

MIT, voir [LICENSE](LICENSE).
