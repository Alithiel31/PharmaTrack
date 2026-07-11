# PharmaTrack — Expression de besoin

## Vision
Outil SaaS accessible à distance pour l'industrie pharmaceutique, permettant de
retrouver rapidement des informations sur les composants/pièces d'équipements
industriels — des données aujourd'hui souvent cataloguées mais peu accessibles
sur le terrain.

## Besoin principal
- Rechercher un équipement/composant via son **code matériel** (référence,
  code interne, code fabricant...).
- Afficher pour ce code :
  - Description de la pièce/équipement
  - Informations de maintenance usuelles (procédure, fréquence, points de
    contrôle)
  - Accès aux plans techniques / schémas / documentation associée

## Idées complémentaires à discuter

### Terrain / usage quotidien
- Scan **QR code / code-barres** sur l'équipement pour lookup instantané
  depuis un mobile (utile en salle blanche, atelier, etc.)
- Mode **hors-ligne (PWA)** pour les zones à connectivité faible
- Interface mobile-first pour les techniciens sur le terrain

### Maintenance
- **Historique des interventions** par équipement (date, technicien,
  observations, pièces remplacées)
- **Planification préventive** avec alertes (email/SMS) avant échéance
  d'entretien ou de calibration
- Suivi des **certificats de calibration** avec dates de validité

### Conformité pharma (GxP)
- Traçabilité complète des modifications (audit trail) — souvent exigé en
  environnement GMP
- Gestion de versions sur les documents (plans, procédures) avec historique
  des révisions
- Piste pour signature électronique / conformité 21 CFR Part 11 si le
  produit doit être utilisé en environnement validé

### Gestion documentaire
- Stockage de fichiers (PDF, plans CAO, manuels constructeur, notices)
- Recherche par mots-clés, catégorie, fabricant, ou référence équivalente
  (cross-reference entre fournisseurs)

### Pièces détachées
- Inventaire des pièces de rechange liées à chaque équipement
- Liens fournisseurs / informations d'approvisionnement (souvent un point
  de friction cité par les clients de ce secteur)

### SaaS / architecture
- **Multi-tenant** (plusieurs sites ou entreprises clientes isolées)
- Gestion des rôles (technicien, responsable maintenance, qualité/audit,
  lecture seule)
- API d'import/export pour interfacer avec un CMMS/ERP existant (SAP PM,
  Maximo...) si le client en a déjà un
- Support multilingue (secteur souvent international)

## Questions ouvertes
- Combien de types d'"items" au départ : équipements complets, pièces
  détachées, les deux ?
- Le produit vise des clients ayant déjà un CMMS (complément) ou doit-il
  remplacer un outil existant ?
- Contraintes réglementaires connues dès le départ (GMP, FDA, ISO 13485...) ?
- Stack technique envisagée ou à définir ensemble (front, back, stockage de
  fichiers, hébergement) ?
- Cible : PME pharma, sous-traitants, ou grands groupes ?

## Statut
Document de travail — première capture du besoin, à affiner au fil des
échanges.
