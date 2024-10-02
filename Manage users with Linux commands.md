# Scenario

In this scenario, a new employee with the username researcher9 joins an organization. You have to add them to the system and continue to manage their access during their time with the organization.

## 1. Add a new user
1. Write a command to add a user called researcher9 to the system.
2. Use the usermod command and -g option to add researcher9 to the research_team group as their primary group.
Adding the user "researcher9" to the system with command "sudo useradd researcher9", then adding that user to the group "research_team" with the command "sudo usermod -g research_team researcher9"<br>
![Add_user_add_group](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/Manager%20Users%20Linux/1.add_user_add_group.PNG)

## 2. Assign file ownership
- The new employee, researcher9, will take responsibility for project_r. In this task, you must make them the owner of the project_r.txt file. The project_r.txt file is located in the /home/researcher2/projects directory, and owned by the researcher2 user.
Changing the ownership of the "project_r.txt", located on "/home/researcher2/projects", to the new user with the "sudo chown researcher9 /home/researcher2/projects/project_r.txt" command. Checking in second img if the permissions were changed.<br>
![change_permission1](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/Manager%20Users%20Linux/2.1.change_permission.PNG)<br>
![change_permission2](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/Manager%20Users%20Linux/2.2.change_permission.PNG)

## 3. Add the user to a secondary group
- A couple of months later, this employee's role at the organization has changed, and they are working in both the Research and the Sales departments. In this task, you must add researcher9 to a secondary group (sales_team). Their primary group is still research_team.
User was added to the "sales_team" group while also been on the primary team using the "sudo usermod -a -G sales_team researcher9" command.<br>
![add_user_secondary_group](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/Manager%20Users%20Linux/3.add_user_secondary_group.PNG)

## 4. Delete a user
- A year later, researcher9, decided to leave the company. In this task, you must remove them from the system.
User was deleted using the "sudo userdel researcher9", but a group with the same name was automatically created, so as a good practice it was deleted (after using the same command without sudo, cause I forgot it) to with the command "sudo groupdeñ researcher9".<br>
![delete_user](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/Manager%20Users%20Linux/4.delete_user.PNG)