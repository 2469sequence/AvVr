# AvVr

Here is our version control repository.
The gitgnore file needs to be placed at the root of your Unity project folder to exclude meta data from pushes to the repo.
1) Figure out how to setup GitHub Desktop app to use for pushing/ pulling versions
2) go to VS installer>modify
 -make sure you have (from the "workloads" section): "Desktop Development with C++" installed
 -make sure you have (from the "individual components"): "Windows 10 SDK.xxx" installed
3)Setup Github "Large File Share" setup correctly
 -type "x64 native tools command prompt for VS 2019" into the windows search bar>run
 -use file explorer to copy address of your git repo where you have the project folder
 -in x64 command prompt: cd "your directory path"
 >see these directions: 
 
 1. Setup Git LFS on your system. You only have to do this once per
    repository per machine:

        git lfs install

 2. Choose the type of files you want to track, for examples all ISO
    images, with git lfs track:

        git lfs track "*.iso"

 3. The above stores this information in gitattributes(5) files, so
    that file need to be added to the repository:

        git add .gitattributes

 3. Commit, push and work with the files normally:

        git add file.iso
        git commit -m "Add disk image"
        git push
