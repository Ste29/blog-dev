1. Create a github repository called <github-username>.github.io
2. Create a folder C:\Hugo\bin
3. Download the Hugo release from https://github.com/gohugoio/hugo/releases (not needed the extended version)
4. Extract the zip into the folder created before (make sure the execuable hugo is with lowercase h)
5. Open CMD, go to Hugo/bin and type `hugo version`
6. To make executable hugo in every folder add bin folder to path variables
7. Go into your dev project folder and run `hugo new site . --force` (if you want you can do everything first in a
dev repo)
8. Add your theme `git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod`
 `git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)`
9. Tell hugo to use the theme: `echo 'theme = "PaperMod"' >> config.toml`
10. Create a new post: `hugo new post/testpage.md`, the generated posts have an header between ---, this stores information to create a render
page. It's some sort of metadata. Those metadata come from archetypes/default.md
11. Every configuration is stored inside config.toml
12. Test your dev repo with `hugo server -D`
13. Set up config.toml (you can use instead config.yaml or config.json, as you pref) https://gohugo.io/getting-started/configuration/
put images in /static
-- 14. commit and push dev repo
-- 15. go in ste29.github.io repo and do `git submodule add -b main https://github.com/Ste29/blog-dev/public` this will clone dev repo in
public folder

14. run deploy.sh in bash or git shell, this will set up your blog
15. copy public folder inside main repo

git remote add origin git@github.com:username/repo.git ---> add a repo to your git project if you didn't start cloning it



-----------------------------------------------

To set url of the repo where everything will be pushed:
`git remote set-url origin https://github.com/Ste29/blog-dev.git`
`git remote set-url origin https://github.com/Ste29/ste29.github.io.git`

To see your current repo link:
`git remote -v`

Same code to link another repo into your dev repo, in particular the main one will be cloned into public folder:
`git submodule add -b main git@github.com:ste29/ste29.github.io public`
`git submodule add -b main https://github.com/Ste29/ste29.github.io public`

First link is for ssh, the second one is for https.
Once the main repo is clone you can run deploy.sh.
The cool thing is that now if you commit from main folder you commit to dev blog repo, if you commit from public/ you commit
to ste29.github.io
In this way you can keep separated commits in your project from commit from linked project. This is useful because sometimes
in your projects you need to incorporate another project.


git submodule copy another repo in a specified folder of your repo, it manages everything through a .gitmodules file and 
modules folder inside .git
Lastly, after deleting a folder commit everything, otherwise things will remain in index file and you will not be able to 
submodule other repo in that folder.

todo: study the deploy script



Interesting blogs: 
- https://youngkin.github.io/post/createafreeblogsite/
- https://solomonmg.github.io/
- https://wowchemy.com/docs/
- https://medium.com/@alessandro.galetto  Obsidian?

configs for papermod:
- https://github.com/adityatelange/hugo-PaperMod/wiki/Installation