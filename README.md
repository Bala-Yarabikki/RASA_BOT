# RASA_BOT

Steps:- 

1. Install 

	sudo apt update
	sudo apt install python3-dev python3-pip

2. check the version : 

	python3 --version
	pip3 --version

3. create virtual env:

	python3 -m venv ./venv

4. Activate virtual env:

	source ./venv/bin/activate

5. again check the version of pip ( anyway we are going to degrade it to 20.2)

	pip3 --version

		output - pip 9.0.1 something.....

6. to make sure pip is updated ( don't worry we are going to change it later)

	pip3 install -U pip

7. install rasa open source

	pip3 install rasa

8. once it is successfully installed . initiate rasa

	rasa init

it will ask you for path give new folder name( /home/bala/rasa/newfolder or somename)
move on by giving Y for multiple times until it say train your model.
to stop training give command : /stop

9. now cd your_newly_created_folder
10. give " rasa train "  it will give the path of your trained model.
11. cross check by giving "rasa shell"
12. stop it by "/stop"
13. give the below command in the same directory of your bot .
:::::::::IMPORTANT ::::: downgrade your pip by giving "pip install --upgrade pip==20.2"

now please confirm the version of pip ( " pip -V ")
it should be 20.2
14. to install Rasa X:

	pip install rasa-x --extra-index-url https://pypi.rasa.com/simple --use-feature=2020-resolver 
15. Now give enable Rasa X

	rasa x
	
	it will automatically prompt to user agreement pdf so 
	just give Y for everything 
	end of it . it will direct you to browser with GUI ( RASA).
ENJOY!
