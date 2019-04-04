<!-- the following links are internal links that links to headers on this page -->
[Getting-started](#getting-started) | [Storage model](#Storage-model) | [Daily workflow](#Daily-workflow) | [Future plan](#Future-plan) | [Need-help](#need-help) | [Contributing](#contributing)

# Welcome to Perfect-Lab-System
<!-- the following visual links (badges) are external links that links other pages than this page -->
[![Read-Wikis](https://img.shields.io/badge/Read-Wikis-brightgreen.svg)](../../wiki)
![Join the chat at https://gitter.im/Perfect-Lab-System/community](https://badges.gitter.im/Perfect-Lab-System/community.svg)](https://gitter.im/Perfect-Lab-System/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![link-to-cloud-storage](https://img.shields.io/badge/Cloud-Storage-yellow.svg)](https://www.google.com/drive/)


<img src="../../blob/master/.github/Images/A-perfect-lab.jpg" align="left" height="250">

I believe a perfect lab would be a lab that **1.Share issues, knowledge, and files in an organized way**; **2.Track every detail of the project**; **3.Automate workflows**

This Perfect-Lab-System project is dedicated to the above goals. This repository is designed as a project template for teamwork in any laboratory (e.g., a Bio-lab). If you want to manage a project with not just code, but also literature, figures, and big data. This repository would be a perfect starting point. Getting started from [here](../../wiki/user-guide#getting-started).

---


## Getting started
- For a new user, please start with the [User-guide](../../wiki/user-guide)
- For an admin user, please start with the [Admin-guide](../../wiki/admin-guide)
- Check the full documentation at [the Wiki page](../../wiki)


## Contributing
Contributions are welcome! Please add issues and make pull requests. There are no stupid questions. All ideas are welcome. This is an experimental project. Be excellent to each other.

If possible, please [read my ideas](./wiki#Design-principles) about this Perfect-Lab-System before you start contributing.


## Need help
- First, please search for solutions in the wiki and GitHub.
- If no solution was found, you can post an issue on this repo.
- Or you can write an email to the system maintainer xxx (example@company.com)

## Storage model
![Storage model](../../blob/master/.github/Images/system-architechture.jpg)

_**One project, one folder.**_

This storage model is for Project-repo and its corresponding local sync folder. (For a Code-repo, Git takes control of everything, no cloud sync involved.)

Since a Project-repo is designed as an online platform, we just use it online, not local usage for this type of repository.

There are two subfolders on GitHub: (.github means these folders are only used on GitHub)
- .github/Images: save images that are rendered in GitHub Wiki
- .github/Files: save files that are linked in GitHub Wiki; for files that larger than 10 MB, please put the files in Nutstore, then paste the links on GitHub

We use sync folders to handle local files that will be shared within a team. The name of the local sync folder should be exactly the same as the corresponding GitHub Project-repo. (For a Code-repo, do not create its sync folder counterpart since Git should take care of everything.)

There are five subfolders inside the sync folder:
- Code folder: You can git clone other Code-repos at here. Since there is no Git control over the sync folder, be sure to put code files in a Code-repo. (If there is no Code-repo, create one for your code. You can name it as `xx-analysis` or `xx-acquisition`.)

- Data folder: Put all experiment data and intermediate data in the **Data** folder. You have the option to auto-sync the data with our storage server. Ask admin users for more info.

- References folder: Put literature and files that are not composed by your team are in the **References** folder. All the files in this folder will be synced via Nutstore with your teammates.

- Results folder: Put the final results for publications such as manuscripts and figures in the **Results** folder. Do not put large data files (>100MB) in this folder since all the files in this folder will be synced via Nutstore with your teammates.

- Working folder: Files in the **Working** folder would not be uploaded or synced with any other devices/services. This is where you put anything unfinished, such as your programs to generate raw data. Please remember to put finished files into the above folders to keep track of them.

Finally, this sync folder will be linked to the corresponding GitHub Project-repo as a badge in README.

### Warnings!
1. **DO NOT ADD ANY FILES/FOLDERS AT THE ROOT OF YOUR SYNC FOLDER**, put the temporary files to the "Working" folder, files to the References folder and the Results folder to auto-sync with Nutstore.
2. **Except the Data, Working folders, DO NOT PUT ANY LARGE FILES (> 100 MB) IN ANY FOLDER**
3. Please do not edit/rename/move/remove the configuration files again.


## Daily workflow
![Diagram-for-daily-workflow](https://github.com/young24/Perfect-Lab-System/blob/master/System/Images/Diagram-for-daily-workflow.jpg)

To make the best use of this perfect lab system, I designed this daily workflow.

## Future plan
- Add a database and link it to this repo
- Add a GitHub bot to do routine checks automatically


> As for myself, I must confess, I am absolutely incapable even of adding without mistakes... My memory is not bad, but it would be insufficient to make me a good chess-player. Why then does it not fail me in a difficult piece of matheatical reasoning where most chess-players would lose themselves? Evidently because it is guided by the general march of the reasoning. A mathematical demonstration is not a simple juxtaposition of syllogisms, it is syllogisms **_placed in a certain order_**, and the order in which these elements are placed is much more important than the elements themselves. If I have the feeling, the intuition, so to speak, of this order, so as to perceive at a glance the reasoning as a whole, I need no longer fear lest I forget one of the elements, for each of them will take its allotted place in the array, and that without any effort of memory on my part.

_- Henri Poincaré on Mathematical Creation_
