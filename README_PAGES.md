Publication de la page via GitHub Pages

1) Le fichier `docs/page_qr_rdiag_ring.html` contient la page à publier.

2) Un workflow GitHub Actions (`.github/workflows/deploy-pages.yml`) est présent :
   - Il déploie automatiquement le contenu du dossier `docs/` sur GitHub Pages à chaque push sur `main`.

3) Pour publier :
   - Commit et push les changements sur la branche `main` :

```bash
git add docs/page_qr_rdiag_ring.html .github/workflows/deploy-pages.yml README_PAGES.md
git commit -m "Add page and GitHub Pages deploy workflow"
git push origin main
```

4) Après le push, GitHub Actions déploiera la page. L'URL sera :
   `https://<owner>.github.io/<repo>/page_qr_rdiag_ring.html` (HTTPS activé automatiquement).

Remarque : si le dépôt a des restrictions (branch protection, actions disabled), activez Actions et Pages dans les settings du dépôt.
