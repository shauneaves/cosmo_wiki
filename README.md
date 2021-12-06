# VUW Cosmogenic Laboratory website
This repository holds the files for the VUW cosmogenic laboratory website.



## How to contribute to this site (for VUW lab users) 
 
1. [**First steps**](#1-first-steps)
    1. [First time editing the webpage?](#first-time-editing-the-webpage)
    2. [Done some editing before?](#done-some-editing-before)
    <br>
2. [**Editing**](#2-editing)
    1. [Add a person](#add-a-person)
        1. [*Change profile photo*](#change-profile-photo)
        2. [*Edit profile page*](#edit-profile-page)
    3. [Add a publication](#add-a-publication)
    4. [Add a project](#add-a-project)
    5. [Edit the documentation](#edit-the-documentation)
    <br>
3. [**Merge changes and submit pull request**](#3-merge-changes-and-submit-pull-request)
-------------

### 1 First steps
_note: this is a work in progress and likely inaccurate_<br>
<br>
You will need
- a [GitHub](https://github.com/) account
- [GitHub Desktop](https://desktop.github.com/)
- a text editor/IDE (notepad will do it, but others offer a bit more, e.g. [VisualCodeStudio](https://code.visualstudio.com/))
We will use the 'fork and pull' method of collaboration from: https://github.community/t/contributing-to-repositories-with-github-desktop/10210

#### First time editing the webpage

- In your web browser, [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repository to create a copy of the source files held in your own GitHub account
- Click the green `Code` button on your forked repository and select `Open in Desktop`: <br>
<p align="center">
  <img src="/assets/media/readme-images/open-with-github-desktop.png" />
</p>

- GitHub Desktop will open and maybe ask you where you want to store the cloned files
- It may then ask you how you are planning to use the fork
  - choose **To contribute to the parent project**: <br>

<p align="center">
  <img src="/assets/media/readme-images/how-are-you-planning-to-use-this-fork.png" />
</p>


#### Done some editing before

- Open GitHub Desktop, ensure you are on the `main` branch, and `fetch origin` then `pull` any updates.
- Your local files should now be identical with this repository and you are ready to make more edits.

-------------
### 2 Editing
The webpages are written in Markdown, a very simple markup language that is quick and easy to learn. <br>
   > ***Useful markdown tips and tricks***
   > *Here are some resources:*
   > - [Good overview of Markdown](https://www.markdownguide.org/)
   > - [Embed a custom Google Map](https://tribulant.com/blog/wordpress/easy-embedding-a-google-map-with-multiple-markers-to-your-site/)
<br>

- In GitHub Desktop, click the `Current branch` dropdown and then click `New branch`. Give it your new branch an intuitive name for your edits (e.g. '*adding-person*', or '*adding-publication*')
- You are now ready to do make some changes to your local files. Things you might like to try are:
  - [Add a person](#add-a-person)
  - [Add a publication](#add-a-publication)
  - [Add a project](#add-a-project)
  - [Edit the documentation](#edit-the-documentation)




#### Add a person

- In your file explorer, navigate to the directory `content/people`
- Create a copy of the `jbloggs` directory and rename it with your first initial and surname (or that of the person you are adding)


##### Change profile photo

- In your new directory, replace `avatar.jpg` with a profile picture for the new person. Note: this file must be named `avatar.jpg`

##### Edit profile page

- Open the file `_index.md`, which holds the content for the profile page. It comprises several sections; most are self explanatory (e.g. `title`, `role`, etc) and/or have some further explanatory comments in the code
  -  `education`: you can add more qualifications by adding more `course:`, `institution:`, `year:` triplets for each qualification.
  -  `social`: similarly, multiple social media accounts can be represented by repeating `icon:`, `icon_pack:`, `link:`.
     -  learn more about icons [here](https://wowchemy.com/docs/getting-started/page-builder/#icons)
  - `user_groups:` choose the relevant user group for the person by replacing the [] with one of the following (note failure to do this will mean the person is not listed on the 'People' page:
    - Researchers (e.g. academic staff)
    - Grad Students (PhD/MSc/Summer Schol?)
    - Technicians (e.g. professional staff)
    - Visitors
    - Alumni (e.g. former lab members)
- once you are happy with your edits, follow [these instructions](#merge-changes-and-submit-pull-request) to merge your changes and submit them to be added to the website source files


#### Add a publication

- Open `content/pubs/_index.md` in your chosen text editor
  - This file holds all of the content for the [publications page of the website](https://sad-jennings-c7dd2d.netlify.app/pubs/)
- Publications are listed alphabetically by year of publication.
- The webpage makes use of the [HTML details element](https://gist.github.com/scmx/eca72d44afee0113ceb0349dd54a84a2), which makes dropdowns for a cleaner appearance 
- This effect is producted using the following code:

```
<details>
  <summary>2022</summary>
- __Author, A., Author, B. YEAR__. [Article title](Article DOI URL). _Journal title_ Volume(issue). Pages. 
</details>
```

- Paste your publication reference into the correct alphabetical location for the relevant year
- Format the entry to be consistent with the current style, e.g.
  - __bold author names__
  - [hyperlinked article title](https://www.doi.org/)
  - _italic journal title_
- When finished adding publications save your changes to `content/pubs/_index.md`
- Once you are happy with your edits, follow [these instructions](#merge-changes-and-submit-pull-request) to merge your changes and submit them to be added to the website source files



#### Add a project

_instructions coming_

#### Edit the documentation

_instructions coming_


-------------
### 3 Merge changes and submit pull request
*not yet accurate* <br>
[Source guide](https://github.community/t/contributing-to-repositories-with-github-desktop/10210)

- In the GitHub Desktop client, commit your changes with a short descriptive message: <br>
<p align="center">
  <img src="/assets/media/readme-images/commit-changes.png" />
</p>

- Now switch to the **main** branch.
- Click **Repository > Pull** in GitHub Desktop to ensure the main branch is up to date with the remote repositories
<p align="center">
  <img src="/assets/media/readme-images/pull-from-upstream.png" />
</p>

- Go to **Branch > Compare to branch** and select your edited branch.
- If there are no merge conflicts, then click **Create a merge commit** to update the main branch
<p align="center">
  <img src="/assets/media/readme-images/compare-to-branch-and-merge.png" />
</p>


- You can begin the the process of creating a *pull request* within GitHub Desktop by going to the menu and selecting **Branch > Create Pull Request**
  - this opens a *pull request* window in your browser
  - provide a written description of your edits and then click **Create pull request**
  - GitHub will then send your suggested changes to Netlify that will check for errors.
  - If the website will not deploy with your edits, then you will see someting like the following:
    <p align="center">
      <img src="/assets/media/readme-images/pull-request-netlify-fail.png" />
    </p>

    - In this case, check the error messages for details and then repeat the editing steps (edit branch, commit, merge with main) to address the issue(s)
    - When you merge with the main branch, GitHub will autmatically update your pull request
    - Hopefully you will then see a success message, e.g.
      <p align="center">
        <img src="/assets/media/readme-images/pull-request-netlify-pass.png" />
      </p>

    - You can see how the website will look once your changes are accepted by clicking the :sunglasses:**Browse the preview** url


<br>
<br>
------------------

### Make your own website:
This website is built using the [Wowchemy-Hugo-Research Group theme](https://github.com/wowchemy/starter-hugo-research-group). This repository holds the source files that are connected to [netlify](https://www.netlify.com/), which deploys the website front end. LEarn more about this general approach:
- 👉 [**Get Started**](https://wowchemy.com/hugo-themes/)
- 📚 [View the **documentation**](https://wowchemy.com/docs/)
- 💬 [Chat with the **Wowchemy community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
