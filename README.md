in the current development conda env.
 make sure the script works.
 
set file structure, in anaconda terminal 
python setup.py sdist bdist_wheel

this will create a folder and 2 files in if succeed.
remove not unnecessary files in the dist folder( old version) and upload only succeeded verion 

python -m twine upload dist/*

this will ask your pypi login info ,


in any new enviroment or other machine

python -m pip install test_deploy_package==1.0.8
it will create an exe in the following location ( on the other systerm, might be a bin)
c:\programdata\anaconda3\scripts\test_deploy.exe

test_deploy.exe --a=test_deploy.csv will get the result

__init__.py is empty
readme.md, and other doc can be empty too

