# py-test-auto-framework

Sample Test Automation project to show automation by using Python, Pytest and Selenium in Page Object Model structure. 

## Prerequisite

* Python 3.7 +
* pipenv should be installed (follow instruction here https://github.com/pypa/pipenv)


## Installation
```bash
git clone https://github.com/st-mn/py-test-auto-framework.git
```
```bash
cd py-test-auto-framework
```
```bash
virtualenv venv
```
```bash
source venv/bin/activate
```
```bash
pip install -r requirements.txt
```
```bash
export PYTHONPATH=$(pwd):$PYTHONPATH
```


## To Run Test

```python
#to run all test
pytest -v
```
```python
#to run all test and generate html report
pytest --html=report.html -v
```
```python
#to run test function containing keyword (registration
pytest -v -k registration
#to run test function marked with mentioned marker (positive)
pytest -v -m positive


```

* Root directory contains docker-compose file to run selenium hub and node. Running it and changing value of "environment" to "remote" in tests> config_test.json.
* Complete site's Pom and Tests should be placed inside site name folder - AutomationPractice > Module name - registration_and_login > then pom, tests, testdata.
* testdata folder contains the Test Data Provider class and maintaining created account details as well.
