
### 1. Make code changes


In git bash, type
```bash
cd ~/ron2015schmitt.github.io
git pull origin main'
code .
```
 edit code
   
### 2. Run website locally

In git bash, type
```bash
bundle exec jekyll serve --watch –-livereload
```
<img width="881" height="194" alt="image" src="https://github.com/user-attachments/assets/3e8a4639-fdad-478b-a775-90bf813c3d0e" />

Click on the link listed.

When done, quit via Ctrl-C

### 3. publish changes

First execute the following locally in git bach
```bash
bundle exec jekyll clean
bundle exec jekyll build
```
Then commit and push the changes to github.

### 4. Force rebuild of site

```bash
curl -u ron2015schmitt:token -X POST https://api.github.com/repos/ron2015schmitt/ron2015schmitt.github.io/pages/builds -H "Accept: application/vnd.github.mister-fantastic-preview+json"
```

For more information refer to [Force github to rebuild](https://federicoterzi.com/blog/how-to-force-github-pages-to-rebuild-jekyll-website/)

### 5. Verify changes


[ron2015schmitt.github.io](https://ron2015schmitt.github.io/)
