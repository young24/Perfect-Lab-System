<!-- the following links are internal links that links to headers on this page -->
[Getting-started](#getting-started) | [Storage model](#Storage-model) | [Daily workflow](#Daily-workflow) | [Future plan](#Future-plan) | [Need-help](#need-help) | [Contributing](#contributing)

# Welcome to Perfect-Lab-System
<!-- the following visual links (badges) are external links that links other pages than this page -->
[![Read-Wikis](https://img.shields.io/badge/Read-Wikis-brightgreen.svg)](../../wiki)
[![Join the chat at](https://badges.gitter.im/Perfect-Lab-System/community.svg)](https://gitter.im/Perfect-Lab-System/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![link-to-cloud-storage](https://img.shields.io/badge/Cloud-Storage-yellow.svg)](https://www.google.com/drive/)


<img src="../../blob/master/System/Images/A-perfect-lab.jpg" align="left" height="250">

I believe a perfect lab would be a lab that **1. Share issues, knowledge, and everything in an organized way**; **2. Track every detail of the project**; **3. Automate workflows**

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
- Or you can write an email to me (bysin7@gmail.com)

## Storage model
![Storage model](../../blob/master/System/Images/system-architechture.jpg)

_**One project, one folder**_

This storage model is for Project-repo.

There are two subfolders only displayed on GitHub: (.github means these folders are only used on GitHub)
- .github/Images: save images that are rendered in GitHub Wiki
- .github/Files: save files that are linked in GitHub Wiki

There are five subfolders
- **Code**: put all your code files here (including jupyter notebook etc.) However, please do not save the generated figures in this folder (save them in the Results folder). You can also link a separate code repo with "git submodule" ([see details](https://git-scm.com/book/en/v2/Git-Tools-Submodules))

- **Data**: Put all experiment data and intermediate data in the **Data** folder. For big data, only put links here.

- **Docs**: Put binary files, such as WORD, powerpoint here. Do not recommend put too many paper here. My suggestion is using a cloud paper management and only put notes on Wiki. For one or two Google Docs (cloud-based sync files), one can use gitignore to ignore the files in git control

- **Results**: Put the final results for publications such as manuscripts and figures in the **Results** folder. Do not put large data files (>100MB) in this folder since all the files in this folder will be synced via Nutstore with your teammates.

- **Working**: Files in the **Working** folder will not be uploaded or synced with GitHub or any other service. It's like a sandbox for you to experiment (e.g., write a new application). Please remember to put finished files into the above folders so that git can track them.

### Warnings!
1. **DO NOT ADD ANY FILES/FOLDERS AT THE ROOT OF YOUR SYNC FOLDER**; put the temporary files in the "Working" folder


## Daily workflow
![Diagram-for-daily-workflow](../../blob/master/System/Images/Daily-workflow.jpg)

To make the best use of this perfect lab system, I designed this daily workflow.

## Future plan
- Add a database and link it to this repo
- Add a GitHub bot to do routine checks automatically
- Update this system with GitHub repo template
- Write a section of privacy statement


> As for myself, I must confess, I am absolutely incapable even of adding without mistakes... My memory is not bad, but it would be insufficient to make me a good chess-player. Why then does it not fail me in a difficult piece of matheatical reasoning where most chess-players would lose themselves? Evidently because it is guided by the general march of the reasoning. A mathematical demonstration is not a simple juxtaposition of syllogisms, it is syllogisms **_placed in a certain order_**, and the order in which these elements are placed is much more important than the elements themselves. If I have the feeling, the intuition, so to speak, of this order, so as to perceive at a glance the reasoning as a whole, I need no longer fear lest I forget one of the elements, for each of them will take its allotted place in the array, and that without any effort of memory on my part.

_- Henri Poincaré on Mathematical Creation_
