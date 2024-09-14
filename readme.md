# Home work 2

## Procedure Followed

	1. Setup Python in my local system WSL using the below commands
		```bash
		sudo apt update -y
		sudo apt install python3-pip
		pip3 --version
		```
	2. Cloned the git hub repository provided to the local using below command.
		```bash
		git clone git@github.com:kaw393939/git_python_testing_setup_homework.git
		```
	3. Installed the required packages and Tested the cloned code using below commands.
		```bash
		source venv/bin/activate <- activates the virtual environment.
		pip3 install -r requirements.txt
		pytest --pylint --cov
		```
	4. Created a new folder myproject and created a virtual env (venv) inside the myproject folder.
		```bash
		mkdir myproject
		cd myproject
		virtualenv venv
		source ./venv/bin/activate
		```
	5. Installing the python dependencies using pip and used freeze to create requirements.txt.
		```bash
		pip3 install pytest pytest-pylint pytest-cov
		pip3 freeze > requirements.txt
		pip3 install -r requirements.txt
		```
	6. Created the "tests" and "calculator" folders with its respective "__init__.py files in them.
		```bash
		mkdir tests calculator
		cd tests
		vi __init__.py <- enter the content given and saved.
		cd..
		vi __init__.py <- enter the content given and saved.
		cd ..
		```
	7. Added the other test files .gitignore .pylintrc pytest.ini 
		```bash
		vi .gitignore
		vi .pylintrc
		vi pytest.ini
		-- Added the content from the repo given and saved.
		```
	8. Added the code to the test_calculator.py file. Successfully completed testing using below commands.
		```bash
		pytest
		pytest --pylint
		pytest --pylint --cov
		```
	9. Completed the commit operations and Pushed to the origin repository.
		```bash
		git init
		git remote add origin --SSHurl of repository--
		git checkout -b FilesAdded
		git add <all the pendingfiles>
		git commit -m "Comments"
		git push origin FilesAdded
		```
	10. Created a git pull request on github and pulled all the latest changes to the repository.
	11. Updated the local branch with the remote changes
		```bash
		git pull --rebase origin master
		```

