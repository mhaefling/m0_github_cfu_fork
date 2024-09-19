| git command | Usage | Notes | 
| ----------- | ----------- | ----------- |
| `git init` | Initialize the scanning and monitoring of the directory it is called in. | Be careful of which directly you call this command in | 
| `git add <filename>` | Adds that file to the "staging" area of the git repository and awaits the users commitment to the changes made to that file. | This will not commit changes to the repository |
| `git commit -m "Message Here"` | Submits the changes to the git repository with a message attached that should follow a standard practice of: | "This commit will..." "Explain the updates that were made" to the file(s) you're commiting. |
| `git status` | Will display the status of the current get repository such as: | (a.) modified files that have not been added to the staging area. (b.) files that have been added to the staging area but have not yet been submitted with a commit. (c.) clean working "tree" or directory structure with no modifications. |
| `git diff` | Provides detailed differences made to a file from the last time that it was added to the staging area or committed to the repository. | Changes will be displayed in green text in the CLI |
| `git log` | Provides a list of changes made to the repository | Authors Name, Email, Date, Time, hashed commit id value. |
| `git remote -v` | Provides details of current connection to github | This can confirm if you're connected in general to the github cloud and if you're connected via https or ssh. | 
| `git remote remove` | This will disconnect your connection to the github cloud repo | This can be used if you connected via https by mistake or if you accidently cloned someone elses repo and need to fork it and reconnect to your repo |
| `git remote add origin <ssh key>` | Used to connect to a github cloud repo via ssh | Always better to connnect via ssh than https as secure shell (SSH) uses better cryptographic algorithms. Although RSA isn't the greatest. |
| `git branch -M main` | Declares the directly you're in on your local machine as the main branch on the cloud repo. | Main branch is the root directory of you cloud repo |
| `git push -u origin main` | "Pushes" / Uploads all modified files | Files remain on your local machine but are copied to the github cloud repo, just in case your local files were to get corrupted |