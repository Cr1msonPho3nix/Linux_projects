# Scenario

In this scenario, you must examine and manage the permissions on the files in the /home/researcher2/projects directory for the researcher2 user.
The researcher2 user is part of the research_team group.
You must check the permissions for all files in the directory, including any hidden files, to make sure that permissions align with the authorization that should be given. When it doesn't, you must change the permissions.

## 1. Checking file and directory details
1. Navigate to the projects directory.
2. List the contents and permissions of the projects directory.

Moving to the specified directory and checking all files's permissions (even hidden ones) with "ls -la" command.<br>
![Checking_file_permissions](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/File%20Permission/1.Checking_file_permissions.PNG)

## 2. Change file permissions
1. Check whether any files in the projects directory have write permissions for the owner type of other.
Checking "project_k.txt" permissions and removing "write" permission in it.<br>
![Checking_file_permissions](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/File%20Permission/2.Remove_permission_project_k.PNG)

## 3. Change file permissions on a hidden file
1. Change the permissions of the file .project_x.txt so that both the user and the group can read, but not write to, the file.
Checking permissions of the hidden file ".project_x.txt", removing "write" and adding "read" permissions to group.<br>
![Change_permission_hidden_file](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/File%20Permission/3.change_permission_hidden_file.PNG)

## 4. Change directory permissions
1. Remove the execute permission for the group from the drafts directory.
Checking "drafs" directory and removing "execute" permission in it.<br>
![Remove_directory_permission](https://github.com/Cr1msonPho3nix/Linux_projects/blob/main/img/File%20Permission/4.Remove_directory_permission.PNG)

