GIT:- Free and Open source version control system 
Version control :- Management of changes to documents, computer programs, large websites, and other collections of informations 

Terms 
- Directory - Folder 
- Terminal or command line - Interface for Text commands 
- CLI - Command Line Interface
- cd - Change directory
- Code Editor - Word processor for writing code
- Repository - Project or folder/place where your project is kept
- Github - A website to host your git repositories online 
- Git - is a tool that track the changes in your code over time 



GIT COMMANDS

- Clone - Bring a repository that is hosted somewher like Github into a folder on your local machine 

    -- git clone https://github.com/debolek/python-script-to-fetch-the-commit-history-and-index-all-commits-in-Elastic-Search.git
    
    ![GIT CLONE](https://user-images.githubusercontent.com/37187773/140627899-9aeba8f1-41ff-4772-b689-bb9f19d0849b.jpg)
    

- add - Track your files and changes in GIT in case you make any changes 

   git add .      
-git init
- git status 
   

   ![git status](https://user-images.githubusercontent.com/37187773/140627977-1d866a0f-897f-4039-9e83-552ef52bd5e1.jpg)

   
- commit- save your files in GIT
      commits to a remote repo, like GITHUB 

     git commit -m "Added python-script-to-fetch-the-commit-history-and-index-all-commits-in-Elastic-Search" -m "some description"
    
    ### m is the message 

![git commit](https://user-images.githubusercontent.com/37187773/140628140-75603682-1e21-426c-b56a-1a0f24daca74.jpg)

- Push - Upload GIT
    To push to git you need to configure the ssh keygen. There are two keys the one with.pub is the public one that you will put on github while the one without is       your private one and must not be shared with anyone 

![ssh key generation](https://user-images.githubusercontent.com/37187773/140642226-bc00b899-8f23-4445-a967-709a820befe7.jpg)
    
     git push origin master 
     
     git remote and add origin git@github.com:debolek/devopsreference.git
     
     git remote -v  
     
     git push -u original master               ###-u is setupstream  if you add it then next time you will not need to use original master,you will just put git push 


- Pull - Download changes from remote repo to your local machine, the opposite of push 


    ####### GIT WORK FLOW ############
    
    ![commit2](https://user-images.githubusercontent.com/37187773/140642628-9340adfe-5f03-40cc-842a-38b12e9e467e.jpg)


    ![local workflow](https://user-images.githubusercontent.com/37187773/140642630-d5ed3f52-18af-4af8-bee0-9cf24ba938f0.jpg)
    
    
    
    
   GIT BRANCHING 
   
   ![GIT BRANCHING](https://user-images.githubusercontent.com/37187773/140642685-269682eb-66f6-480e-95fa-c2c45641c38c.jpg)
   
   

  ![GIT BRANCHING 2](https://user-images.githubusercontent.com/37187773/140642690-6e759872-8e4e-4411-bbf4-56b0d20362ad.jpg)
  
  
  
  
 ![concept of branching](https://user-images.githubusercontent.com/37187773/140642985-e295433b-9a4c-4c32-b0ef-12eafa8247eb.jpg)
 
 
    git branch
    git checkout     ###to switch between branches or check out 
    
    git checkout -b 'feature-readme-instruction'    ##-b is to create a new branch with a new name
    git branch       ##you will see the new branch you created 
    git checkout master
    git branch
    git checkout feature-readme-instructions
    
    
    if you modify your file 
    git status 
    git add ReadME.md
    git commit -m "update readme"
    git checkout master 
    
    git diff        ##diff will show changes that have been made to the two files 
    git merger feature-readme-instructions
    git checkout feature-readme-instructions
    git status 
    git push -u origin feature-readme-instructions
    
    
    
    
    
    
    
    
