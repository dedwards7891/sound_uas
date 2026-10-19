HOW TO UPDATE THE SOUND UAS JEKYLL WEBSITE

1. Open VS Code.

2. Open a terminal.

3. Navigate to the website folder:

   cd C:\Users\Edwards\sound_uas

4. Start the local Jekyll server:

   bundle exec jekyll serve

5. Open the local website in a browser:

   http://127.0.0.1:4000/sounduas/

6. Make any desired changes to site files:
   - index.md (home page)
   - about.markdown (About page)
   - _config.yml (site settings)
   - _posts\ (blog posts)
   - images and other assets

7. Save files and refresh the browser.
   Jekyll automatically rebuilds when files are saved.

8. When finished testing, stop the server:

   Ctrl+C

9. Check what files have changed:

   git status

10. Add the changes:

   git add .

11. Commit the changes:

   git commit -m "Describe the update"

   Example:

   git commit -m "Update homepage"

12. Push changes to GitHub:

   git push origin gh-pages

13. Wait a few minutes for GitHub Pages to publish the update.

14. Verify the live site:
    https://sounduas.com

TROUBLESHOOTING

If the site does not update locally:

   bundle exec jekyll clean
   bundle exec jekyll serve

If Git rejects a push:

   git pull origin gh-pages

Complete the merge if prompted, then:

   git push origin gh-pages

COMMON FILES

Home page:
   index.md

Site settings:
   _config.yml

Blog posts:
   _posts\

About page:
   about.markdown

Custom domain:
   CNAME