# Link With Buyers — GitHub Pages review build

This is a self-contained, two-page static site:

- `/` — the complete sales page
- `/schedule/` — the Calendly booking page (`https://calendly.com/pgai`)

## Publish with GitHub Pages

1. Create a new GitHub repository and upload the contents of this folder to its default branch.
2. In **Settings → Pages**, choose **Deploy from a branch**, then select the default branch and `/ (root)`.
3. In **Custom domain**, enter `linkwithbuyers.com`. The included `CNAME` file should remain at the site root.
4. In Porkbun, point the domain to GitHub Pages following GitHub’s current custom-domain instructions. Add the `www` host as well, then choose one version of the site as the canonical redirect destination.
5. Enable **Enforce HTTPS** in GitHub Pages once its DNS check completes.

The canonical URLs, sitemap, robots file, social metadata, and structured data are already prepared for `https://linkwithbuyers.com/`.

## Notes

- The source images collected from the current public page are stored locally in `assets/`; the build does not rely on Gamma code or hosted templates.
- Calendly is intentionally the only external runtime dependency. The booking page includes a direct-link fallback if the embedded calendar is blocked.
- Before going live, replace or add an Open Graph share image if you have a preferred brand asset.
