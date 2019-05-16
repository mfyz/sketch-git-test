# sketch-git-test

Plain Git Sketch Experiment


1) Open Terminal, navigate to desktop and create new folder with running command below:

```
cd ~/Desktop
mkdir sketch-git-test
cd sketch-git-test
```

2) Then create a simple single artboard, few layers sketch file and save it inside this folder.

3) Download and save download.sh and upload.sh files from https://github.com/ahuk/sketch-collaboration to the sketch-git-test folder.

4) Open and edit both download and upload sh files with defining your sketch files without the file extension to be processed like:

```
files="design"
```

5) Create the git repository and add github/gitlab remote configuration:

```
git init
git remote add origin git@github.com:mfyz/sketch-git-test.git
```

Start pushing updates and use download script to sync latest versions

```
# to upload changes with a message
sh upload.sh new rectangle added

# to download the latest changes
sh download.sh
```
