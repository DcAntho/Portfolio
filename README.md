# Portfolio — Anthony Da Costa

Portfolio one-page cinématographique : une rangée de pochettes en **coverflow 3D**
(perspective, inclinaison, reflet au sol), une intro vidéo, une musique de fond,
et une page dédiée par projet.

## Stack
HTML / CSS / JavaScript **vanilla**, sans framework. Police Helvetica + IBM Plex Mono (labels).

## Structure
```
index.html              → home (coverflow)
projects.js             → données des projets (partagé), titres / images / liens
apropos.html            → à propos
contact.html            → contact
projets/<nom>/index.html→ page détaillée par projet (poz, mapch, animalia, j42,
                          danse, flirty, joecoaching, horschamp)
media/                  → vidéos & images (par projet)
```

## Lancer en local
Un serveur statique suffit (les routes en `/dossier/` ne marchent qu'avec un serveur,
pas en `file://`) :
```bash
python3 -m http.server 4599
# puis http://localhost:4599
```

## Éditer les projets
Tout se règle dans `projects.js` : `title`, `cat`, `year`, `img` (capsule),
`grad` (fallback), `glow`, `url` (page du projet).
