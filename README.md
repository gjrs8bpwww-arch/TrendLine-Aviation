# Trendline Aviation website

Single-page website for Trendline Aviation LLC. Reliability analytics and CASS support.
Live at https://www.trendlineaviation.com

## Files

- `index.html`: the complete website (HTML, CSS and JavaScript in one file)
- `CNAME`: connects the site to www.trendlineaviation.com
- `404.html`: simple "page not found" page
- `robots.txt` and `sitemap.xml`: help search engines find the site
- `.nojekyll`: tells GitHub Pages to serve the files as-is

## 1. Publish with GitHub Pages

1. Create a new repository on GitHub (for example `trendline-aviation`).
2. Upload all the files in this folder to the repository root (including `CNAME` and `.nojekyll`).
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then **Save**.
5. Under **Custom domain**, make sure it shows `www.trendlineaviation.com` and click **Save**.

## 2. Set up DNS at your domain registrar

Add these records (replace `your-username` with your GitHub username):

| Type  | Name / Host | Value                     |
|-------|-------------|---------------------------|
| CNAME | www         | your-username.github.io   |
| A     | @           | 185.199.108.153           |
| A     | @           | 185.199.109.153           |
| A     | @           | 185.199.110.153           |
| A     | @           | 185.199.111.153           |

The CNAME record points www.trendlineaviation.com to GitHub. The A records make
trendlineaviation.com (without www) redirect to the www address.
Remove any old A or CNAME records for `@` or `www` that point somewhere else.
Always confirm the current values in GitHub's documentation: "Managing a custom domain for your GitHub Pages site".

## 3. Turn on HTTPS

DNS changes can take from a few minutes up to 24 hours. Once GitHub shows the domain
as verified in **Settings → Pages**, tick **Enforce HTTPS**.

## Editing

All content is in `index.html`. Contact email: HR@trendlineaviation.com.
Re-check the eCFR and FAA links in the CASS section periodically, since regulations can change.
