# pytest-demo
This is a pytest framework demo.

### Folder Structure
```
pytest-demo
    │  README.md
    │
    ├─libs
    │      module.py
    │      __init__.py
    │
    └─tests
           test_module.py
```

### Install pytest
```
pip install pytest
```

### Module & test
- Define a class named Module in `module.py`.  
- In `test_module.py`, import the class Mudule, and define test functions. Adds the "test" prefix to every name.  
-  Add the project path (pytest-demo) to the environment variable `PYTHONPATH`.  

Edit `.bashrc` profile; paste the line at the end: 

```
vim ~/.bashrc 
```
```
export PYTHONPATH="${PYTHONPATH}:/foo/pytest-demo"
```

Source the bashrc profile when run your code.  

```
source ~/.bashrc
```

### Test
Test `Module.get_true()` returns True, and `Module.get_false()` returns False.  

cd to the project path (pytest-demo) and run:
```
pytest

```
or more details run `pytest -v`.
 