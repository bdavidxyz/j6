<div align="center">

  # Chirpy Jekyll Theme

  A minimal, responsive, and feature-rich Jekyll theme for technical writing.

</div>

## Current changes

- using chirpy version 6.4.1
- tools-version set to ruby 3.2.2 / nodejs 18.20.2
- renamed pages-deploy.yml.hook to pages-deploy.yml

removed 

      - name: Test site
        run: |
          bundle exec htmlproofer _site \
            \-\-disable-external=true \
            \-\-ignore-urls "/^http:\/\/127.0.0.1/,/^http:\/\/0.0.0.0/,/^http:\/\/localhost/"

after action "Build site"
from pages-deploy

  - set baseurl