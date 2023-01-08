---
layout: home
title: "Setup Staff Site" 
parent: "Instructor Setup"
nav_order: 2
---

<style>
 summary { 
     border: 4px solid #9CBEBE;
     padding: 0.5em;
     background-color:  #DAE6E6;
     margin-bottom: 0.5em;
 }

 summary p {
  margin: 0px;
  padding 0px;
  display: inline-block;
 }
    
 details { 
    margin-top: 0.5em;
    margin-bottom: 0.5em;
    margin-left: auto;
    margin-right: auto;
    width: 95%;
    border: 4px solid #047C91;
    padding: 0.5em;
 }
</style>

# {{page.title}}

To set up a staff site like this one for your course:

1. Identify a source staff site; perhaps the one you are reading now.  We'll need the URL of that site, e.g. `git@github.com:ucsb-cs16/w23-staff.git`
2. Create your own new empty repo under the appropriate course organization, e.g. `ucsb-cs16/s23-staff`
3. Clone that repo at command line, e.g. 
   ```
   git clone git@github.com:ucsb-cs16/s23-staff.git
   ```
4. cd into the newly created directory
   ```
   cd s23-staff
   ```
5. Add a remote for the source repo:
   ```
   git remote add source git@github.com:ucsb-cs16/w23-staff.git
   ```
6. Copy from the `main` branch of the source repo, and push to the new repo:
   ```
   git checkout -b main
   git pull source main
   git push origin main
   ```
7. Enable GitHub Pages using GitHub Actions workflows.
   - Navigate to Settings, then Pages
   - Under **Build and Deployment**, on the dropdown menu, select `GitHub Actions`
   
   <img width="382" alt="image" src="https://user-images.githubusercontent.com/1119017/211215037-6ff49245-b7ed-4ff4-b26f-57efb2432ee7.png">

   <img width="1305" alt="image" src="https://user-images.githubusercontent.com/1119017/211214987-a3afa97b-6289-437b-914f-9e30a177a2b0.png">

8. Your pages should now build.
9. Edit `_config.yml` and change the places that the quarter is referred to, especially these lines:

   ```
   ...
   title: "CS16 W23 Staff"
   baseurl: '/w23c-staff' # the subpath of your site, e.g. /blog
   ...
   gh_edit_repository: "https://github.com/ucsb-16/w23-staff" # the github URL for your repo
   ```
   
   You may also want to edit the parts of the file that provide the navigation links at the top of the page, i.e. everything nested under `aux_links`

Your page should now be available online on GitHub pages.

---------

For attribution, please keep the reference to the author:

> Content developed and released under the CC BY 4.0 by Phill Conrad.

If you would like us to add or correct anything in these instructions, feel free to use the `edit this page on GitHub` link below and then submit a Pull Request from your forked repo.

