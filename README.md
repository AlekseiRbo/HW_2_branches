# HW_2

1. On the local repository, make branches for:  
  * Postman        `git branch Postman`
  * Jmeter         `git branch Jmeter`
  * CheckLists     `git branch CheckLists`
  * Bag Reports    `git branch BagReports`
  * SQL            `git branch SQL`
  * Charles        `git branch Charles`
  * Mobile testing `git branch MobileTesting`

2. Push all branches to an external repository  
  `git add .`  
  `git commit 'Add branches'`  
  `git checkout main`  
  `git push -u origin 'Postman' 'Jmeter' 'CheckLists' 'Bag_Reports' 'SQL' 'Charles' 'MobileTesting'`  

3. In the Bag Reports branch, make a text document with the bug report structure   
  `git checkout Bag_Reports`  
  `vim bug_report.txt`    
```
ID: 001  
Title: What? Where? When?  
Severity: Medium  
Priority: High
Precondition: Preparation steps  
Environment: Devices  
STR: Steps to reproduce  
ER: Expected Result  
AR: Actual Result  
Attachment: link  
```
4. Push the bug report structure to an external repository  
  `git add .`  
  `git commit -m "Add bug_report.txt"`  
  `git push`  

5. Merge the Bag Reports branch into Main  
  `git checkout main`  
  `git merge Bag_Reports`  

6. Push main to external repository  
  `git add .`  
  `git commit -m "merge BagReports"`  
  `git push`  

7. Sketch the checklist structure in the CheckLists branch  
  `git checkout CheckLists`  
  `vim check-list.txt`  
```
ID
Title
Status
Link
```
8. Push structure to external repository  
  `git add .`  
  `git commit -m "Add check-list.txt"`  
  `git push`  

9. On an external repository, make a *Pull Request* of the **CheckLists** branch in main      
Go to [GitHub_AlekseiRbo](https://github.com/AlekseiRbo/HW_2_branches/ "GitHub_AlekseiRbo") , click **Compare & Pull request**  

10. Synchronize External and Local branches Main  
  `git checkout main`  
  `git fetch`  
  `git pull`  
  
