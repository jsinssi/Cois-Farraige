# Cois Farraige Holistic Therapies — website

A "coming soon" page for Mary Butler's reflexology and Reiki practice: the logo
and the words "Website coming soon". It is plain HTML and CSS, with no build step,
so it runs on GitHub Pages as it is.

```
index.html            the page
assets/css/styles.css styles
assets/images/        logo, favicons and the social sharing image
DESIGN.md             brand colours and fonts
```

## Preview on your computer

From this folder, run:

```bash
python -m http.server 8642
```

Then open http://localhost:8642.

## Publish on GitHub Pages

1. Create a new repository on GitHub, for example `cois-farraige`.
2. Push this folder to it:

   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/cois-farraige.git
   git push -u origin main
   ```

3. On GitHub, open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then branch
   **main** and folder **/ (root)**, and click **Save**.
5. After a minute or two the page is live at
   `https://YOUR-USERNAME.github.io/cois-farraige/`.

### Use the coisfarraige.net domain

1. In **Settings → Pages → Custom domain**, enter `coisfarraige.net` and save.
2. At the domain registrar, set these DNS records:
   - `A` records for `coisfarraige.net` pointing to `185.199.108.153`,
     `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
   - a `CNAME` record for `www` pointing to `YOUR-USERNAME.github.io`
3. Once the domain shows as verified, tick **Enforce HTTPS**.

The social sharing image in `index.html` points to coisfarraige.net, so link
previews show the logo once the domain points here.
