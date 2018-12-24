## Short-cuts 
[Project's wiki](https://github.com/young24/Perfect-Lab-System/wiki). This link is provided for an easier access from the mobile end.

# Welcome to the perfect lab system
![The perfect lab](https://github.com/young24/Perfect-Lab-System/blob/master/System/Images/diagram-for-the-perfect-lab-system.jpg)

What I want to do is to develop a perfect project management system for labs (typically, bio-labs) which is able to 
1. Share issues, knowledge, and files in an organized way.
2. Track every detail of the project and quantify the contribution of each member.
3. Automate workflows.

## The ideal storage model
![The ideal storage system](https://github.com/young24/Perfect-Lab-System/blob/master/System/Images/Diagram-for-system.jpg)

_**One project, one folder.**_

The left column represents the local project folder structure which has five sub-folders. For these subfolders:

First, the code folder stores codes that will be uploaded directly to GitHub.

Second, the data folder stores all raw data, and any other intermediate data, analysis results except results that will be shown in publications. Files in this folder would be backed up to the private server while pointers to files would be uploaded to GitHub to track all files with GitHub. However, deleting operation to the data files in the local folder would not delete the data on the private server. It is up to users that whether modifications to the local data should be updated to the ones on the private server.

Third, the results folder stores all results of the project which will be presented on publications. No large data files (>100 MB) should be put into this folder. Files in this folder would also be uploaded to the cloud storage where project members can access them even outside the school while pointers to files will be uploaded to GitHub to keep track of files. It would be better to automatically open external applications when click on some files in GitHub. For example, click on a MS Word file to open the online Word processer to read it. Maybe MS programmers would do this for me since MS has already bought GitHub.

Fourth, the reference folder stores all references from others than team members. The major file type would be PDF. Ideally, there would be a reference list written in Markdown where registered every document in the Reference folder. And only this reference list would be uploaded to GitHub while the real documents would be uploaded to a shared space that every member can access through one click on the item in the reference list even they are not in school. However, the current solution is as the same as the one for the results folder.

**Best Practice for the reference folder?**: add a link to the web library (e.g., Mendeley's) in a Markdown file. So that people can go to the shared library by just one click on GitHub.

Fifth, the working folder holds everything else in the process such as programs in use and data generated from the experiment system. Nothing would be uploaded to GitHub neither in the hard-copy way nor the pointer-copy way.

## Daily workflow
![Diagram-for-daily-workflow](https://github.com/young24/Perfect-Lab-System/blob/master/System/Images/Diagram-for-daily-workflow.jpg)

To make the best use of this perfect lab system, I designed this daily workflow in which "Trellow + Unito" provides seamless support on the mobile end. 

## Future plan
- Integrate Git-LFS in this system. There are still some technical issues to deal with. 
- Integrate one of the reference managers to deal with references in a more efficient way.
- Incorporate all actions/manipulations into the Git framework.



> As for myself, I must confess, I am absolutely incapable even of adding without mistakes... My memory is not bad, but it would be insufficient to make me a good chess-player. Why then does it not fail me in a difficult piece of matheatical reasoning where most chess-players would lose themselves? Evidently because it is guided by the general march of the reasoning. A mathematical demonstration is not a simple juxtaposition of syllogisms, it is syllogisms **_placed in a certain order_**, and the order in which these elements are placed is much more important than the elements themselves. If I have the feeling, the intuition, so to speak, of this order, so as to perceive at a glance the reasoning as a whole, I need no longer fear lest I forget one of the elements, for each of them will take its allotted place in the array, and that without any effort of memory on my part.

_- Henri Poincaré on Mathematical Creation_




