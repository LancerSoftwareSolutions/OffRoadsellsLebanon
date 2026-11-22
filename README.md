# Off Roadsells Lebanon: setup notes

## index.html
Edit only the five settings at the top of the file (also explained in the note at the top of the file):
- `SECRET_ROUTE`: your secret admin path
- `ADMIN_PASSWORD`: the admin password
- `GITHUB_OWNER`: your GitHub username
- `GITHUB_REPO`: the repository name
- `GITHUB_BRANCH`: usually `main`

Nothing else needs changing.

## cars.json
Holds the car listings. You don't need to edit it by hand. The admin page rewrites it when you press **Publish to website**.
- The two sample cars (Polaris and Can-Am) are placeholders. Delete them in the admin page before going live.
- Don't add comments or extra fields to this file. It must stay a plain list of cars, or the site won't load it.

## cars/ (photos)
Created automatically by the admin page when photos are uploaded. Don't rename or move these files, or the car cards will lose their pictures.

## logo.png
The logo, used as the browser tab icon. No changes needed.

## Upload
Put all files at the top level of the GitHub repository, then turn on GitHub Pages (Settings → Pages → Deploy from a branch → main → /root).
