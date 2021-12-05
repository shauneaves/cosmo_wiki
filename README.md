# VUW Cosmogenic Laboratory website
This repository holds the files for the VUW cosmogenic laboratory website.


## How to contribute to this site (for VUW lab users) 

_note: this is a work in progress and likely inaccurate_<br>
<br>
You will need
- a [GitHub](https://github.com/) account
- [GitHub Desktop](https://desktop.github.com/)
- a text editor/IDE (notepad will do it, but others offer a bit more, e.g. [VisualCodeStudio](https://code.visualstudio.com/))

### 1 First steps

We will use the 'fork and pull' method of collaboration from: https://github.community/t/contributing-to-repositories-with-github-desktop/10210

#### First time editing the webpage?
- In your web browser, [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repository to create a copy of the source files held in your own GH account
- Open GitHub Desktop and clone the forked repository from your GitHub account
  - this creates a local copy on your hard disk
- In GitHub Desktop, click the 'Current branch' dropdown and click 'New branch'. Give it a name.
- You are now ready to do make some changes, things you might like to try are:
  - [Add a person](#add-a-person)
  - [Add a publication](#add-a-publication)
  - [Add a project](#add-a-project)
  - [Edit the documentation](#edit-the-documentation)

#### Done some editing before?
- You will need to [sync your fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) to ensure it is up to date
- Then in GitHub Desktop 

### 2 Editing

#### Useful markdown tips and tricks

- [Good overview of Markdown](https://www.markdownguide.org/)
- [Embed a custom Google Map](https://tribulant.com/blog/wordpress/easy-embedding-a-google-map-with-multiple-markers-to-your-site/)

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

_instructions coming_



#### Add a project

_instructions coming_

#### Edit the documentation

_instructions coming_


### 3 Merge changes and submit pull request






## Make your own website:
This website is built using the [Wowchemy-Hugo-Research Group theme](https://github.com/wowchemy/starter-hugo-research-group). This repository holds the source files that are connected to [netlify](https://www.netlify.com/), which deploys the website front end. LEarn more about this general approach:
- 👉 [**Get Started**](https://wowchemy.com/hugo-themes/)
- 📚 [View the **documentation**](https://wowchemy.com/docs/)
- 💬 [Chat with the **Wowchemy community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
