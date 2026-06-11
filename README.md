# Holy Crew Signup Page

Live site for Holy Crew, the high school student leadership program of Mannahouse Youth.

## Deploy with GitHub Pages (no terminal needed)

1. Go to github.com and click the + in the top right, then New repository.
2. Name it holy-crew, set it to Public, click Create repository.
3. On the new repo page, click "uploading an existing file".
4. Drag index.html (and this README) into the upload box, click Commit changes.
5. Go to Settings > Pages. Under Branch, pick "main" and "/ (root)", click Save.
6. Wait about a minute. Your page is live at https://YOURUSERNAME.github.io/holy-crew/

## Connect crew.mannahouse.org (optional)

1. In Settings > Pages > Custom domain, type crew.mannahouse.org and Save.
2. In the Wix DNS dashboard for mannahouse.org, add a CNAME record:
   Host: crew    Value: YOURUSERNAME.github.io
3. Wait for DNS to update (minutes to a few hours), then check Enforce HTTPS in GitHub Pages settings.

## Wire the signup form

1. Follow the setup steps at the top of holy-crew-signup-handler.gs (Google Sheet + Apps Script).
2. Open index.html, find SIGNUP_ENDPOINT near the bottom, paste your Apps Script web app URL between the quotes.
3. Re-upload index.html to the repo (Add file > Upload files > drag > Commit). Pages redeploys automatically.
