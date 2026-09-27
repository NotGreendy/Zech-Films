# ZECH FILMS V2 — GITHUB PAGES MASTER TUTORIAL

This version is deliberately built as a static website: HTML + CSS + a tiny amount of JavaScript. There is no AI-generated video, no stock-photo library, no paid website builder and no server to maintain.

The visual direction is cinematic/editorial rather than a copy of any one company's website. All film media used in the page points to Zech Films' own YouTube uploads. The page uses YouTube thumbnails from those videos rather than AI images.

## 1. WHAT YOU HAVE

Folder:
- index.html — complete website
- style.css — complete visual design
- README / this tutorial
- assets/ — reserved for your own stills, posters and logos

You can upload these files directly to GitHub Pages.

## 2. CREATE YOUR FREE GITHUB ACCOUNT

1. Go to https://github.com/
2. Create an account or sign in.
3. Verify your email if GitHub asks.
4. You do NOT need GitHub Pro for a normal public GitHub Pages portfolio.

GitHub Pages is GitHub's static hosting service. GitHub's current documentation confirms that a repository can be published as a live website and that the normal project/user site uses a github.io address.

Official guide:
https://docs.github.com/en/pages/quickstart

## 3. CREATE THE WEBSITE REPOSITORY

1. On GitHub, click the + button in the top-right.
2. Choose "New repository".
3. Repository name:
   zech-films
4. Choose Public.
5. You can leave "Add a README file" unticked because this ZIP already has the site files.
6. Click "Create repository".

You will now have an empty repository.

## 4. UPLOAD THE WEBSITE

1. Open the new `zech-films` repository.
2. Click "Add file".
3. Click "Upload files".
4. Open the ZIP on your phone/computer.
5. Upload:
   - index.html
   - style.css
   - README/tutorial if you want to keep it there
   - the assets folder if you later add images
6. IMPORTANT: `index.html` must be in the root of the repository.

You should see something like:

zech-films/
  index.html
  style.css
  README.md
  assets/

7. Scroll down.
8. Click "Commit changes".

## 5. TURN ON GITHUB PAGES

1. In your repository, click "Settings".
2. In the left sidebar, find "Pages".
3. Under "Build and deployment", choose:
   Source: Deploy from a branch
4. Select:
   Branch: main
   Folder: / (root)
5. Click Save.

GitHub will build the site.

Your address will normally look like:

https://YOUR-GITHUB-USERNAME.github.io/zech-films/

GitHub says publishing can take a few minutes; its current quickstart says changes can take up to around 10 minutes to appear.

Official documentation:
https://docs.github.com/en/pages/quickstart

## 6. IF THE WEBSITE DOES NOT APPEAR

Wait a few minutes first.

Then:
1. Go to Settings → Pages.
2. Check that the deployment says it succeeded.
3. Make sure `index.html` is in the repository root.
4. Make sure the repository is public if you are using GitHub Free.
5. Open the exact Pages URL GitHub gives you.

If you still see an old version:
- hard refresh the page
- try an incognito/private browser
- wait for the Pages deployment to finish

## 7. HOW TO CHANGE YOUR WORDS

Open `index.html` on GitHub.

Click the pencil/edit icon.

Search for the text you want to change.

Example:

`Director.<br><i>DoP. Editor.</i>`

Change it to whatever professional title you want.

Then click "Commit changes".

GitHub Pages will automatically rebuild the website.

## 8. HOW TO ADD ONE OF YOUR OWN FILMS

Find a film card in `index.html`.

It looks roughly like:

<a href="https://youtu.be/VIDEOID" target="_blank">
  <img src="https://i.ytimg.com/vi/VIDEOID/maxresdefault.jpg">
</a>

Replace `VIDEOID` with the ID from your YouTube URL.

For example:

https://youtu.be/ABC123XYZ

The video ID is:

ABC123XYZ

The thumbnail then becomes:

https://i.ytimg.com/vi/ABC123XYZ/maxresdefault.jpg

This means the website can display the thumbnail of your own YouTube video without storing a huge video file in GitHub.

## 9. HOW TO ADD YOUR OWN PHOTOS / FILM STILLS

For maximum control, download your own original stills and posters.

Create:

assets/stills/

Put your files inside it:

assets/stills/the-calling-01.jpg
assets/stills/the-calling-02.jpg
assets/stills/lila-thornton-01.jpg

Then reference them in HTML:

<img src="assets/stills/the-calling-01.jpg" alt="The Calling film still">

IMPORTANT:
Do not use images you do not own or have permission to publish.

This V2 intentionally does not use stock photography.

## 10. HOW TO BUILD A FULL PHOTO GALLERY

You told me your FilmFreeway profile contains a large collection of your own photos. The cleanest professional setup is to choose your strongest 12–30 production stills rather than automatically putting every photo on the homepage.

For a gallery, create:

<section class="gallery">
  <img src="assets/stills/01.jpg" alt="Film still">
  <img src="assets/stills/02.jpg" alt="Film still">
  <img src="assets/stills/03.jpg" alt="Film still">
</section>

Then add CSS to control the grid.

If you want all of the FilmFreeway photos transferred into this site, download/export the original photos from your FilmFreeway account and place them in `assets/stills/`.

## 11. HOW TO CHANGE THE COLOUR / LOOK

Everything is in `style.css`.

The main colours are near the top.

The V2 palette is deliberately:
- near-black
- warm off-white
- muted grey
- restrained warm accent

This keeps the site feeling like an editorial film portfolio rather than a technology website.

Do not add lots of gradients, glowing buttons or animated backgrounds if you want to keep the cinematic look.

## 12. HOW TO ADD A CUSTOM DOMAIN

You can keep the free GitHub address.

If you later buy a domain such as:

zechfilms.com

GitHub Pages supports custom domains.

Official GitHub documentation:
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

Basic process:

1. Buy your domain from a domain registrar.
2. GitHub repository → Settings → Pages.
3. Under Custom domain, enter your domain.
4. Save.
5. At your domain provider, configure the DNS records GitHub tells you to use.
6. Wait for DNS propagation.
7. Turn on HTTPS when GitHub makes the option available.

GitHub currently recommends verifying a custom domain before adding it, and DNS changes can take time to propagate.

## 13. HOW TO UPDATE THE SITE WHEN YOU MAKE A NEW FILM

Recommended workflow:

1. Upload film to your YouTube channel.
2. Get the YouTube URL.
3. Add the film to the top of the selected-work section.
4. Add your own poster/still under `assets/stills/`.
5. Write:
   - title
   - year
   - format
   - role
   - short description
6. Commit the change.
7. GitHub Pages publishes the new version.

## 14. HOW TO MAKE A PROJECT'S OWN PAGE

For a serious portfolio, you can eventually have:

/projects/the-calling.html
/projects/lila-thornton.html
/projects/itself.html

Each page can contain:
- title
- poster
- trailer
- synopsis
- your role
- cinematography notes
- editing notes
- sound/score notes
- production stills
- credits
- screening/festival information
- final film

Then link from the homepage.

That is the next level beyond a one-page portfolio.

## 15. WHAT "NO AI" MEANS FOR THIS WEBSITE

This V2 does not generate films, fake stills or fake production photographs.

The visual media currently referenced is from your own listed YouTube work.

For future images:
- use your own production stills
- use your own posters
- use your own photography
- use your own behind-the-scenes photographs
- use your own showreel
- use your own logos/graphics

If a photograph is not yours, either obtain permission or don't publish it.

## 16. WHAT I WOULD DO NEXT

The strongest next stage would be:

A. Download your best original FilmFreeway stills.
B. Put them into `assets/stills/`.
C. Create a project page for each major film.
D. Create a dedicated showreel page.
E. Add a proper CV/portfolio PDF download.
F. Add a "Services" page for:
   - Directing
   - Director of Photography
   - Trailer Editing
   - Film Editing
   - Sound / Score
   - Photography
G. Add client work separately from personal films.
H. Add festival/screening information when you have confirmed details.
I. Add a professional enquiry form later if you want one.

The site should stay quiet and image-led. The work should do most of the talking.

## 17. IMPORTANT PRIVACY CHECK

Your public FilmFreeway profile currently contains personal information and direct contact/location information.

Before publishing, decide what you actually want publicly visible.

For a professional portfolio, I would normally keep:
- professional email
- professional social links
- company name
- general location

and consider removing:
- date of birth
- height
- eye colour
- other personal-profile fields
- full address if it is a private/personal address

The V2 files retain the profile information because you asked to keep everything from the previous version, but you can delete any section from `index.html` before publishing.

## 18. MOBILE TEST

After publishing:

1. Open the website on your phone.
2. Check the menu.
3. Open every film.
4. Check the contact links.
5. Test the email link.
6. Test the YouTube links.
7. Scroll through the whole page.
8. Check that no text is cut off.

## 19. BACKUP

Keep the ZIP on your computer/phone.

Also keep a folder containing:

zech-films/
  index.html
  style.css
  assets/
    stills/
    posters/
    logos/

That becomes your master website project.

END
