**This user guide is for new users or users who have little knowledge about GitHub and Perfect-Lab-System. For admin users or experienced users, please check this [Admin-guide](./Admin-guide) to learn more.**

## Why you should use Perfect-Lab-System
Perfect-Lab-System is a [GitHub](#github-and-its-working-flow)-based project managment system, which allows you to
- Share issues, knowledge, and files with lab members in a social and organized way
- Track every details of your projects
- Automate workflows, which can save your time from reporting the project status

In addition, you will save plenty of time in the future if you can spend an hour to learn how the system works. Please start with this [Getting started](#Getting-started). Don't worry, no programming knowledge required.

## Content
- [Getting started](#Getting-started)
- [Programmer guide](#Programmer-guide)
- [Searching function in GitHub](#Searching-function-in-GitHub)
- [Mobile solutions](#mobile-solutions)
- [Add images/files on Wiki](#Add-imagesfiles-on-Wiki)
- [Create relative links to header](#Create-relative-links-to-header)
- [GitHub is social and fun](#Social-is-fun)
- [Markdown](https://guides.github.com/features/mastering-markdown/)
- [Atom editor](#atom-editor)
- [GitHub and its working flow](#github-and-its-working-flow)
- [Work with your local project folder](#Work-with-your-local-project-folder)
- [Real life scenarios that GitHub can help you](#Real-life-scenarios-that-GitHub-can-help-you)
- [Build a personal website with GitHub](#Build-a-personal-website-with-GitHub-GitHub-Pages)

## Getting started
Welcome to Perfect-Lab-System. In this guide, you'll learn how to use Perfect-Lab-System to
- Make your life easier, less stressful, more organized
- Work with your teammates and boss efficiently

First, you have to do some preparations. Since it's super easy, you can do the following preparations by yourself.

### Preparations
1. Create a GitHub account, better use your name as username.
2. Upload your photo and edit the profile with your name. Click [here](https://github.com/settings/profile) to start. Note down your username and email.
3. Create a cloud storage account (e.g., Google Drive). Note down your username and email.
4. Tell the admin user your GitHub and Nustore username&email to sign you into the Wenlab organization.
5. Learn GitHub-flavored Markdown language in 5 minutes. You will use this grammar everyday, such as post an [issue](https://help.github.com/en/articles/about-issues) and write a [Wiki](https://help.github.com/en/articles/about-wikis) on GitHub. Click [here](https://guides.github.com/features/mastering-markdown/) to start.
6. Excellent job. You are prepared.

Then, you need some practice to learn how to use this Perfect-Lab-System in your everyday workflow. Please call an admin user (any one in the [admin-team](https://github.com/orgs/Wenlab/teams/admin-users)) to assist you to complete the following tasks.

### Practice
_This practice introduction inherits the style from [Angular tutorial](https://angular.io/tutorial)._

This practice covers the fundamentals of Perfect-Lab-System.
In this tutorial you will complete several tasks that will frequently be used in the future.

By the end of the tutorial you will be able to do the following:
- Write a Markdown file
- Post your request/question/suggestion as an issue on GitHub
- Note down a protocol/experiment note as a Wiki on GitHub
- Insert a picture in your issue/Wiki
- Link a file at the sync folder in your issue/Wiki
- Create a internal link that linked to headers of the same file
- Create a badge (visual link) to external files/website
- Create a QR code for your protocol with the Intelligent-Protocol template
- Create a README for your Project-Repo with the Project-repo template
- Find a file/wiki/issue/anything on GitHub through searching
- Add an emoji to a comment to indicate your agreement/attitude
- Create a voting with emojis
- Manage notications of GitHub and the cloud service
- Gain enough confidence to do whatever you want

You'll learn enough Perfect-Lab-System to get started and gain confidence that Perfect-Lab-System can do whatever you need it to do.

Let's get started. Please ask the admin user to help you
- Build up a repository for your project or sign you in an existing project.

This repository will be your [Project-Repo](TODO:link-to-explanation). Also, ask the admin user to initiate a local sync folder for your project on your working computer. Please **do not edit the GitHub repository name** since it might corrupt links related to the repositories.

- Save a bookmark of [the Wenlab GitHub dashboard](https://github.com/orgs/Wenlab/dashboard) in your browser.


**Please do all the practice on the repository of Perfect-Lab-System. Create a new branch with your name before starting.**
#### Task1 - create an issue
Post an issue is the best way to get others' attention to people. You are going to create an issue to tell the lab you start using Perfect-Lab-System.
- Click on the `Issues` tab
- Before you create an issue, please search if there are already similar issues
  - in the search bar, delete all filters, search `I YOUR-NAME start using Perfect-Lab-System`, replace `YOUR-NAME` with your true name.
  - No results matched? Great, no one has the same name as you.
- Strike on that big green button to create a new issue
  - Get started with `I'm in!!!`
  - Change the title to `I YOUR-NAME start using Perfect-Lab-System`, replace `YOUR-NAME` with your true name.
  - Edit the content with your information and photo.
  - Submit new issue
  - Add a `happy` emoji to the comment, click on the face button on the upper-right corner. You can also let people vote in this way.
  - On the right, you may see settings of `Assignee`, `Label`, and other interesting things. Feel free to give it a try.
- Excellent! You've posted your first GitHub issue.

#### Task2 - create an README file
This time, you are going to create a README.md file to introduce your project.
If you don't know what your project is, please ask the lab head afterwards. Anyway, we can start with a simple project - **Project-X**.
- First, there's a README.md in your repository. Delete everything in that file
- Then, you need to create a main section to describe your project
  - Copy the following content to the README file:
  ```
  # Welcome to PROJECT-X
  This Project-repo is about xxx. Please leave your issues and wikis here. There is no stupid questions or silly notes. Be excellent to each other in the team.
  ```
  - Replace `xxx` with `neuroscience and creativity`
- There are some websites you might need to access everyday. Let's add each one as a visual link - a GitHub badge.
  - Add the following code to the end of README file
  ```
  [![badge-name](link-to-badge)](link-to-the-webpage)
  ```
  - Create a static badge at [shields.io](https://img.shields.io).
    - Enter `Check` at label
    - Enter `Wenlab-Admin` at message
    - Select `red` as the badge color
    - Make Badge
    - Replace `link-to-badge` in README file with the link of the badge
  - Open the lab dashboard in a new tab
    - Right-click on the Administration repo
    - Copy link address
    - Replace `link-to-the-webpage` in README file with the link
  - Great. You've created a visual badge to a webpage. Click the `Preview` tab to check it out
  - Create another badge for the corresponding sync folder
    - Tip: you can get the address in web mode
- Then, create another section to introduce your teammates, objectives, plan, code dependencies, and more
  - Add the following code to the end of README file
  ```
  - [Person-A](link2person-A-profile-page): responsibilies
  - [Person-B](link2person-B-profile-page): responsibilies
  - [Person-C](link2person-C-profile-page): responsibilies

  ## Objectives
  1. objective1
  2. obj2
  3. obj3

  ## Plan
  1. Step1
  2. Step2
  3. Step3

  ## Code dependencies
  - [Code-repo1](link2code-repo1)
  - [Code-repo2](link2code-repo1)

  ## More
  ```
  - Edit the content with the actual info. `Code dependencies` are those Code-repos you'll need for your project. If you don't know some of the content, just leave them there.
- Finally, you need to create a top navigation panel to link to the headers you just created
  - Add the following code to the **beginning** of README file
  ```
  [People]() | [Objectives]() | [Plan]() | [Code dependencies]() | [More]()
  ```
  - In the Preview mode, when you move the mouse to a header, there will be a link symbol. Right-click on it and copy the address
  - Copy the link to corresponding bracket
  - Remove the part before `#`
  - Awesome. You just learned how to create a relative link to internal headers.

Now, you've got a pretty decent project introduction page - _README.md_.

#### Task3 - create a wiki
Another important thing you'll do on GitHub is to document your experiment notes and protocols in Wiki. Let's create a Wiki page to start.

- Click on the `Wiki` tab, then strike on the green button to create a new Wiki page
- Enter `YOUR-NAME Experiment Perfect-Lab-System practice` as the title, replace `YOUR-NAME` with your name
- Copy the following code and edit the content with the actual info, you don't need to edit the badges.
  ```
  # Exeperiment name
  Note everything about _EXPERIMENT_ at here.

  [![SUBJECT website](https://img.shields.io/badge/Check-website-red.svg)](link-to-a-website)
  [![References Lib](https://img.shields.io/badge/Check-references-blue.svg)](link-to-references-lib)
  ```
- Then create a `Content list` for your wiki
  - Copy the following code at the end of the content
  ```
  ## Content list
  - [item1](#item1)
  - [protocol1](#protocol1)

  ## item1

  ### Part 1 about item1

  This is a table for two formulas:

  |     | A (50 ml) | B (100 ml) |
  | --- | --------- | ---------- |
  | X   | 1/2       | -1/2       |
  | Y   | -1/2      | 1/2        |

  ### Part 2 about item1
  ## protocol1

  [Step1-xx](#step1-xx) | [Step2-xx](#step2-xx) | [Step3-xx](#step3-xx)

  ### Step1-xx

  ### Step2-xx

  ### Step3-xx

  ### Details/explanations
  ```
  - Notice that we use internal links to link to headers of this wiki
  - There is a table which you can edit to document a schedule or a formula.
  - Also, there is a quote format that you use to insert words from others.
  - What if you want to insert an image? This is different from inserting images in Wiki. You can't drop in images directly. So what should you do?
    - Put the image to `.github/Images/`, just drop them in through browser
    - Right-click to get the link to the image
    - Copy the link to the markdown link
    - Now, click the preview to check if the image is rendering

Great. You are a master of Markdown now.

#### Task4 - manage notifications and other settings
In the last task, you'll learn how to manage notifications and other settings to help you avoid extra stress.

- Click on your avatar, then select `Settings` in the drop-down menu.
- Select `Notifications` in the right panel.
- Then, it's up to you how you'd like to receive notications from GitHub. Also, for each repository, you can choose `unwatch` to stop receiving notifications unless you are being mentioned. For each issue, you can opt out notifications by selecting `not receive notifications on the right panel`
- For Nutstore, you can uncheck `Show notification on files updated` in Settings. TODO: update this with Google Drive.
- Also, you can choose to [receive notifications through mobile](#Mobile-solutions) or [RSS](https://blogtrottr.com/confirm/BLqd0X).

#### Task5 - work-with-your-local-project-folder
Please start with [this tutorial](#Work-with-your-local-project-folder).


Congratulations! You have learned all necessary knowledge and skills to use Perfect-Lab-System. However, even the best method requires practice. Please try to practice this working style everyday (e.g., post an issue to ask a question about Perfect-Lab-System). If you want to learn more, please [check the content table](#content-table) to find out topics that interest you. For programmers **(have independently written a script with more than 20 lines)**, please turn to [Programmer guide](#Programmer-guide) to learn more.

In the future, for your everyday work,
- if you have an issue to solve, such as a bug to report, a feature to request, a problem unsolved, please **post an issue** to your Project-repo. However, make sure you have already checked the README and wiki pages of the repository since all important info should be noted at these places.

- If you have some protocols to follow every day/interesting findings/experiment notes, please **note them down to Wiki** of the most relevant repository. You can use Markdown to [insert an image or link a file](#Add-imagesfiles-on-Wiki) in your Wiki pages.



### Notices
- Please **do not edit the repository names** since it might corrupt links related to those repositories.


## Programmer guide
**You are assumed to be finished with [Getting started](#Getting-started). If not, please start with [Getting started](#Getting-started) first.**

```
Imagine a scenario that you are going to add a new feature to an existing program. However, you still want the original program functions as usual - i.e., you cannot modify the code directly. What would you do? Copy the code, modify it, and then paste it back?
```

[GitHub flow](https://guides.github.com/introduction/flow/) offers a better solution. Please take 5 minutes to read this powerful workflow design: [GitHub flow](https://guides.github.com/introduction/flow/).

Additionally, as a programmer, you must learn Git and use it everyday. Git is a version control system that GitHub is based on. If you don't accept this claim, please have a look of these posts: [New Developer? You should’ve learned Git yesterday.](https://codeburst.io/number-one-piece-of-advice-for-new-developers-ddd08abc8bfa); [4 Reasons Why Beginning Programmers Should Use “Git”](https://medium.com/swlh/git-as-the-newbies-learning-steroid-963a2146220b).

I recommend you to start with [GitHub Learning Lab](https://lab.github.com/githubtraining/introduction-to-github) which is an interactive way to teach you things without leaving GitHub. However, there are some alternatives:
- [tutorialspoint](https://www.tutorialspoint.com/git/) - a great website to learn Git basics

Finally, please download and use Atom - a 21st-century hackable editor which has the full support of Git and GitHub. Start with [this guide](#atom-editor).

Now you are a perfectly equiped programmer who have the power to change the world. If you want to learn more, please [check the content table](#content-table) to find out topics that interest you.

## Mobile solutions
Use your browser to check GitHub is the recommended solution. However, there are some Apps available.

- For Android: [OpenHub](https://github.com/ThirtyDegreesRay/OpenHub) and [FastHub](https://github.com/k0shk0sh/FastHub)
- For IOS: [CodeHub](https://github.com/CodeHubApp/CodeHub) and Hubhub which focuses on issues and pull quests.

## Searching function in GitHub
You can use advanced search order in GitHub just like in google.Some useful order:
- `org:`:limit search range,like `org:Wenlab`.
- `repo:`:search in these repositories.
- `created:`:limit the creating-date,like`created:>2019-04-01`
- Or use [advanced search page](https://github.com/search/advanced).
Then use`Ctrl+F` to search in webpage.

## GitHub is social and fun
GitHub is a social APP, which allows you to use emojis and @ to communicate with others. So please be social to make the maximum efficiency of your team.

You can also talk in team (enter your team from the organization). It is just the Wechat group -- instant online communication.

Be social, be verbal, and be communicative.

### Emoji
You can use emoji by enter a ':' in  **Issues** or **Pull requests** or use it in reply.
![use-emoji](https://github.com/Wenlab/Perfect-Lab-System/blob/JJY/.github/Images/use-emoji.jpg)

Also, you can respond to someone's comment by adding emotions from the upper-right corner emotion buttion.

A creative usage of Emoji is that you can use it to vote for something. For example, there is a journal-club issue template that allows people to choose their favourite paper to discuss.

### Notification management
You can change your notication settings at [here](https://github.com/settings/notifications)

## Add images/files on Wiki
### Add files
TODO: write a tutorial with Google Drive.

#### Alternative solution (Do not recommend)
Drop the files into the .github/Files folder directly.

### Add images
For online pictures,copy the URL to embed pictures just like what you learned in [GitHub-flavored Markdown language](https://guides.github.com/features/mastering-markdown/).

For local pictures, drag and drop image file into the writing text box in **Issues** or **Pull requests** to upload your image.

TODO: simplify this part, just drop in images.
![upload-image](https://user-images.githubusercontent.com/5516900/28625071-70c1dbee-721b-11e7-8154-0dab00e37583.png)

Then you will get a URL like `![image2](https://user-images.githubusercontent.com/5516900/28625071-70c1dbee-721b-11e7-8154-0dab00e37583.png)
`which link to your image.

But in **Wiki** it doesn't work.You need first to upload your image to `.github/Images`or upload it by drag and drop image file into the writing text box in **Issues** or **Pull requests**.Then use use the URL like`https://github.com/Wenlab/Perfect-Lab-System/blob/master/.github/Images/Perfect-lab-system-storage-model.jpg` or `https://user-images.githubusercontent.com/5516900/28625071-70c1dbee-721b-11e7-8154-0dab00e37583.png`to embed image.For you can not manage the images you upload to `https://user-images.githubusercontent.com`,uploading to `.github/Images`is probably a safer choice.

## Create relative links to header
1. right-click on the header/file you want to link to
2. copy the link address
3. paste the address into the text, and remove the part before "#"
4. You are all set, do forget to test it to ensure it works.

## Build a personal website with GitHub (GitHub Pages)
People can use GitHub build up personal websites for theirselves or for their projects.
1. [Getting started from here](https://pages.github.com/)
2. A beautiful academic GitHub Pages template: [Academicpages](academicpages.github.io)
3. Build up your personal website with [Academicpages](https://github.com/academicpages/academicpages.github.io). Checkout [the step-by-step guide]()

### Build up your personal website with Academicpages
I modified the tutorial on [Academicpages](https://github.com/academicpages/academicpages.github.io) with more details under MIT License.

1. Fork the repository of [Academicpages](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right.
2. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
3. Set site-wide configuration by editing the file "_config.yml" at the root path.
4. Configure the top menu by editing the file "/_data/navigation.yml"
5. Edit files in "/_pages" folder with the name of the item on the top menu to update the content of each page. (e.g., edit about.md to update the content of your home page.)
6. Update files in "_publications" to update the content of items on the publication page. The same to other pages on the top main menu.
7. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf. Please use [Git LFS](https://git-lfs.github.com/) to track those binaries to keep your repo with a small size.
8. Congratulations! Now, you have your own website through hardwork. Checkout your website at [your GitHub username].github.io (there might be several mins delay after you update the content of your website.)

#### Add a **favicon** to your website tab
> A favicon, a.k.a, a shortcut icon, tab icon, associated with a particular website or web page.

_From [Wikipedia/Favicon](https://en.wikipedia.org/wiki/Favicon)_

If you are interested in creating a favicon for your website, please check the top answer in [this link](https://stackoverflow.com/questions/11488960/how-do-i-put-my-websites-logo-to-be-the-icon-image-in-browser-tabs) to print your icon.


## Atom editor
This editor can render Markdown files in real time, support LaTex grammar, and can even read PDFs. More importantly, it is deeply integrated with Git and GitHub. Therefore, you can use it to perform common Git operations (Click on the Git tab at the lower-left corner).
- Please first check [this blog](https://www.cnblogs.com/fanzhidongyzby/p/6637084.html) to feel the power of this editor.
- Then get to [this link](https://github.atom.io/) to start your pleasant journey with Atom and GitHub.


### Install packages
- Use the apm (Atom Packages Manager) to install packages
  - Usage: in the Windows command prompts (CMD), ``` apm install THE-PACKAGE-NAME ```, replace _THE-PACKAGE-NAME_ with the package name you want to install
- Open the packages manager via `` Ctrl + Shift + P `` open the palette, then search `` install packages `` to open it.

#### Recommended packages
- Markdown-preview-plus: provide LaTeX preview and real-time preview for Markdown
- [goto-definition](https://atom.io/packages/goto-definition): a package allows you to jump to definitions of functions swiftly.
  - 1. ``apm install goto-definition``
  - 2. Download a binary file from [here](https://github.com/BurntSushi/ripgrep/releases)
  - 3. Extract the files to ``C:\Windows\System32\``, then you are all set.

TODO: test those packages and find more

## GitHub and its working flow
TODO: simplify this part

GitHub is an online project managment platform, which makes teams can collaborate in an efficient way. (You alone can be a team too since it usually requires multiple steps to complete a project.)

[GitHub flow guide](https://guides.github.com/introduction/flow/) is the GitHub working flow. If you haven't learned it, please take 5 mins to learn [this brilliant workflow](https://guides.github.com/introduction/flow/).

Then, you can turn to [the official GitHub Guides](https://guides.github.com/) to learn more about GitHub.

If you prefer to watch videos, there are two great introductory videos: (on the Youtube, so you might need some tools to get there.)<br>
1. [GitHub Review • Exploring Workflows](https://www.youtube.com/watch?v=EwWZbyjDs9c&t=3056s)
in which it explains the basic idea of git workflow and how to implement it with Github
2. [Webcast • GitHub for Project Management](https://www.youtube.com/watch?v=6fByt0o4UYs&t=1671s)
in which it explains what the project management is and how to implement it with Github, although it is a little bit outdated.<br>

Find answers to common questions and learn with other GitHub users in the new [GitHub Community Forum](https://github.community)



## Work with your local project folder
![Storage-model](https://github.com/Wenlab/Perfect-Lab-System/blob/master/.github/Images/system-architechture.jpg)

This storage model is for Project-repo and its corresponding local sync folder. (For a Code-repo, Git takes control of everything, no cloud sync involved.)

Since a Project-repo is designed as an online platform, we just use it online, not local usage for this type of repository.

There are two subfolders on GitHub: (.github means these folders are only used on GitHub)
- .github/Images: save images that are rendered in GitHub Wiki
- .github/Files: save files that are linked in GitHub Wiki; for files that larger than 10 MB, please put the files in the sync folder, then paste the links on GitHub

We use sync folders to handle local files that will be shared within a team. The name of the local sync folder should be exactly the same as the corresponding GitHub Project-repo. (For a Code-repo, do not create its sync folder counterpart since Git should take care of everything.)

There are five subfolders inside the sync folder:
- Code folder: You can git clone other Code-repos at here. Since there is no Git control over the sync folder, be sure to put code files in a Code-repo. (If there is no Code-repo, create one for your code. You can name it as `xx-analysis` or `xx-acquisition`.)

- Data folder: Put all experiment data and intermediate data in the **Data** folder. You have the option to auto-sync the data with our storage server. Ask admin users for more info.

- References folder: Put literature and files that are not composed by your team are in the **References** folder. All the files in this folder will be synced via cloud service with your teammates.

- Results folder: Put the final results for publications such as manuscripts and figures in the **Results** folder. Do not put large data files (>100MB) in this folder since all the files in this folder will be synced via cloud service with your teammates.

- Working folder: Files in the **Working** folder would not be uploaded or synced with any other devices/services. This is where you put anything unfinished, such as your programs to generate raw data. Please remember to put finished files into the above folders to keep track of them.

Finally, this sync folder will be linked to the corresponding GitHub Project-repo as a badge in README.

### Warnings!
1. **DO NOT ADD ANY FILES/FOLDERS AT THE ROOT OF YOUR SYNC FOLDER**, put the temporary files to the "Working" folder, files to the References folder and the Results folder to auto-sync with your cloud service (Google Drive).
2. **Except the Data, Working folders, DO NOT PUT ANY LARGE FILES (> 100 MB) IN ANY FOLDER**
3. Please do not edit/rename/move/remove the configuration files again.
