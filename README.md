# GitHub Guide: Creating a Repository with Contributors and Requiring Owner Approval for Code Merges 

## 1. Creating a GitHub Repository 

1. Go to GitHub and log in. 
2. Click on the "+" icon in the top right and select "New repository". 
3. Enter a repository name and select visibility (Public or Private). 
4. Check "Initialize this repository with a README" (optional). 
5. Click "Create repository".
     

## 2. Adding Contributors to the Repository 

1. Go to your repository and click on the "Settings" tab. 
2. In the left sidebar, click "Collaborators and teams". 
3. Under "Manage access", click "Invite a collaborator". 
4. Enter the GitHub username or email of the contributor. 
5. Click "Add collaborator" and send an invite. 
6. The invited contributor must accept the invitation before they can contribute. 

## 3. Setting Up Branch Protection (Requiring Owner Approval) 
1. Go to your repository’s "Settings" tab. 
2. Click "Branches" in the left sidebar. 
3. Under "Branch protection rules", click "Add rule". 
4. In the "Branch name pattern" field, enter main (or your default branch name). 
5. Enable the following:  
  - "Require a pull request before merging". 
  - "Require approvals" (Set required approvals to at least 1). 
  - "Require review from code owners" (Ensures only the owner can approve changes). 
  - (Optional) Require status checks to pass before merging. 
  - Click "Save changes". 

## 4. Setting Up Code Ownership 

To ensure only the repository owner must approve code changes before merging: 

    Create a .github/CODEOWNERS file in the root of the repository. 

    Add the following content: * @ ChlioP 

    This makes the repository owner the mandatory reviewer before merging any code. 

## 5. How Contributors Can Access the Repository 

Once added as a collaborator: 

    The contributor should accept the invitation sent to their GitHub account. 

    Clone the repository locally using:  

git clone https://github.com/ChlioP/repo-training 
  

    Navigate into the project directory:  

cd your-repo 
  

## 6. How a Contributor Can Push Changes 

    Create a new branch: git checkout -b feature-branch 
      

    Make changes and commit: git add . 
    git commit -m "Added new feature" 
      

    Push to GitHub: git push origin feature-branch 
      

    Create a Pull Request (PR):  

    Go to the GitHub repository. 

    Click "Pull Requests" → "New pull request". 

    Select feature-branch as the source and main as the target. 

    Click "Create pull request". 

## 7. How the Owner Can Review and Merge Code 

    Go to "Pull Requests" in the GitHub repository. 

    Open the new pull request. 

    Review the changes and leave comments if needed. 

    Click "Approve". 

    Click "Merge pull request" to merge the changes into main. 

    (Optional) Delete the feature-branch after merging. 

## 9. How to access private access to the repo, Please watch this, https://youtu.be/Lhyu_2iLO8w?si=_hGtwn1Fx6Pp-ith 

 

## 9. Resolving merge conflicts 

If a contributor encounters merge conflicts, they need to resolve them manually. Here’s a helpful guide explaining the process step by step: 

https://www.youtube.com/watch?v=HosPml1qkrg 
 
