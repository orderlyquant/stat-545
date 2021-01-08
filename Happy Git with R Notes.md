# Happy Git with R

*notes* and thoughts on [Happy Git with R](https://happygitwithr.com)

## Chapter 9 - Connect to GitHub Account

All went well.

- Took the time to add two-factor authentication to my Github account.
- Setup new Personal Access Token (PAT)
- Did several repo creation, cloning and pushing tests successfully.

## Chapter 10 - Cache Credentials for HTTPS

- decided to standardize all github.com use on HTTPS.
  - JBryan recommendation and Github recommendation
- downloaded and started to use [`credentials`](https://docs.ropensci.org/credentials/)
  package for storage and use of git PAT
- moved the PAT from explicit store in .Renviron to credential lookup in .Rprofile
  using `credentials::credential_helper_set()`

---

*skipping intervening Chapters...walked through all directions, setup is working*

---

## Chapter 15

**New project, GitHub first** is the preferred method because everything gets
setup for pushing/pulling, etc.

The standard setup for creating a new repo on github.com is:

---

![](images/github_first_screen_shot.png)

*note: Add a README file is checked*

---

> There’s a big advantage to the “GitHub first, then RStudio” workflow: the remote
  GitHub repo is added as a remote for your local repo and your local master branch
  is now tracking master on GitHub. This is a technical but important point about
  Git. The practical implication is that you are now set up to push and pull. No
  need to fanny around setting up Git remotes and tracking branches on the command
  line.
  
### 15.4 Push your local changes to GitHub

> This will seem counterintuitive, but first let’s stop and pull from GitHub.
  Establish this habit for the future! If you make changes to the repo in the browser
  or from another machine or (one day) a collaborator has pushed, you will be happier
  if you pull those changes in before you attempt to push.

## Chapter 17 - Existing project, GitHub last

**Important:** this is a key workflow that's a little complicated, so refer to the
[website](https://happygitwithr.com/existing-github-last.html).

