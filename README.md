# project_planning
Repo for notes and planning

link to the packaged project  
https://test.pypi.org/project/funkyAD-funkyADers/0.0.1/

pip install -i https://test.pypi.org/simple/ funkyAD-funkyADers==0.0.1



## Instructions for releasing a new version of the package:

If you have not installed setup tools yet:
	python3 -m pip install --user --upgrade setuptools wheel
	python3 -m pip install --user --upgrade twine

Then:
	- Change setup.py to hold new version number
	- python3 setup.py sdist bdist_wheel
	- python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
	- username: tyleryoo pass: funkyAD207
	- update the version number in README and docs
	- make sure to uninstall the old version (pip uninstall funkyAD-funkyADers) and reinstall the new one before testing
