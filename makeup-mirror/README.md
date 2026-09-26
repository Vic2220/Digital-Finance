# Glow Mirror ✨ — MVP

Miroir de maquillage web pour iPhone :

- **Moitié haute** : un panneau lumineux (comme le flash frontal de Snapchat) qui éclaire ton visage.
  - 4 teintes de lumière : blanc, chaud, froid, rosé
  - 3 niveaux de luminosité (bouton ☀︎)
  - Les boutons se cachent après 3 s pour une lumière 100 % pure — touche la zone blanche pour les réafficher
- **Moitié basse** : la caméra frontale en mode miroir, avec zoom 1× / 1.5× / 2×.
- L'écran reste allumé (Wake Lock) tant que le miroir est ouvert.

100 % HTML/CSS/JS, aucun build, aucune dépendance.

## Utiliser sur iPhone

La caméra ne fonctionne qu'en **HTTPS**. Le plus simple : GitHub Pages.

1. Sur GitHub : **Settings → Pages → Source : Deploy from a branch**, choisis la branche et le dossier `/ (root)`.
2. Ouvre `https://<ton-user>.github.io/<repo>/makeup-mirror/` dans Safari.
3. Touche **Activer le miroir** et autorise la caméra.
4. Astuce : **Partager → Sur l'écran d'accueil** pour l'avoir en plein écran comme une vraie app.
5. Mets la luminosité de l'iPhone au maximum pour un meilleur effet flash.

## Tester en local

```bash
cd makeup-mirror
python3 -m http.server 8000
# ouvre http://localhost:8000 (localhost est autorisé pour la caméra)
```
