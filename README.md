# How to run an automation test in Pytest in incognito mode on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=Pytest-incognito)

If you want to run you automation test in Pytest in incognito mode on Lambdatest, you can use the following steps to upload extension and run your test. You can refer to sample test repo [here](https://github.com/LambdaTest/pytest-selenium-sample).

# Steps:

## Step 1: Add --incognito in browser arguments

In the python file, add the '--incognito' argument to start browser in incognito mode. For example:

```
import pytest
@pytest.fixture
def chrome_options(chrome_options):
    chrome_options.binary_location = '/path/to/chrome'
    chrome_options.add_argument('--incognito')
    return chrome_options
```

## Step 2: Run your test

```
cd tests //navigate to tests directory
python sample_todo.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

