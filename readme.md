# Home work 2

## Procedure Followed

1. Setup Python in my local system WSL using the below commands

		sudo apt update -y
		sudo apt install python3-pip
		pip3 --version

2. Cloned the git hub repository provided to the local using below command.

		git clone git@github.com:kaw393939/git_python_testing_setup_homework.git

3. Installed the required packages and Tested the cloned code using below commands.

		source venv/bin/activate <- activates the virtual environment.
		pip3 install -r requirements.txt
		pytest --pylint --cov

5. Created a new folder myproject and created a virtual env (venv) inside the myproject folder.

		mkdir myproject
		cd myproject
		virtualenv venv
		source ./venv/bin/activate

6. Installing the python dependencies using pip and used freeze to create requirements.txt.

  		pip3 install pytest pytest-pylint pytest-cov
		pip3 freeze > requirements.txt
		pip3 install -r requirements.txt
		
7. Created the "tests" and "calculator" folders with its respective "__init__.py files in them.

		mkdir tests calculator
		cd tests
		vi __init__.py <- enter the content given and saved.
		cd..
		vi __init__.py <- enter the content given and saved.
		cd ..
		
9. Added the other test files .gitignore .pylintrc pytest.ini 

  		vi .gitignore
		vi .pylintrc
		vi pytest.ini
		-- Added the content from the repo given and saved.
		
10. Added the code to the test_calculator.py file. Successfully completed testing using below commands.

		pytest
		pytest --pylint
		pytest --pylint --cov

11. Completed the commit operations and Pushed to the origin repository.

		git init
		git remote add origin --SSHurl of repository--
		git checkout -b FilesAdded
		git add <all the pendingfiles>
		git commit -m "Comments"
		git push origin FilesAdded

12. Created a git pull request on github and pulled all the latest changes to the repository.

13. Updated the local branch with the remote changes

  		git pull --rebase origin master
		


