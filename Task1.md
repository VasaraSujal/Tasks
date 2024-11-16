##### Task 1: Install and Configure Git







##### Task 2: Initialize a Repository

1. first of all create a new folder on desktop

     mkdir new_folder

2. navigate to that folder

    cd new_folder

3. Initialize git 

    git init



#### Task 3: Create a File and Make Multiple Commits

1. Create a new file in this folder with echo command

    echo "new_file" >> new_file.txt

2. Add this file to the stagging area

    git add new_file

3. Add commit to the file

    git commit -m "New commit"

4. Make the change to this file

    echo "make changes" >> new_file.txt

5. add the file to stagging area

    git add new_file

6. Make commit to this file

    git commit -m "Updated text"