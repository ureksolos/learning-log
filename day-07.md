# Day 6

---

- **Date:** 2026-10-30
- **Hours Planned:** 4
- **Hours Achieved:** 6
- **AI Log:** No AI
- **Rebuild result:** Rebuilt test_expense_tracker.py from memory (twice) successfully
- **"The part I'd have to look up tomorrow is:** I think i'd need to study more on pytest.

---


## Pytest Output(s):

### Output 1:

=============================== test session starts ===============================
platform win32 -- Python 3.15.1, pytest-9.2.0, pluggy-1.7.0 -- C:\Users\succe\AppData\Local\Programs\Python\Python315\python.exe
cachedir: .pytest_cache
rootdir: C:\Users\succe\Documents\python-practice
collected 4 items                                                                  

test_expense_tracker.py::test_calculate_total_empty PASSED                   [ 25%]
test_expense_tracker.py::test_calculate_total_single PASSED                  [ 50%]
test_expense_tracker.py::test_calculate_total_multiple PASSED                [ 75%]
test_expense_tracker.py::test_format_expense PASSED                          [100%]

================================ 4 passed in 0.10s ================================


### Output 2(deliberately broken):

=============================== test session starts ===============================
platform win32 -- Python 3.15.1, pytest-9.2.0, pluggy-1.7.0 -- C:\Users\succe\AppData\Local\Programs\Python\Python315\python.exe
cachedir: .pytest_cache
rootdir: C:\Users\succe\Documents\python-practice
collected 4 items                                                                  

test_expense_tracker.py::test_calculate_total_empty PASSED                   [ 25%]
test_expense_tracker.py::test_calculate_total_single FAILED                  [ 50%]
test_expense_tracker.py::test_calculate_total_multiple PASSED                [ 75%]
test_expense_tracker.py::test_format_expense PASSED                          [100%]

==================================== FAILURES =====================================
___________________________ test_calculate_total_single ___________________________

    def test_calculate_total_single():
>       assert calculate_total([{"desc" : "food", "amount" : 12.5}]) == 13
E       AssertionError: assert 12.5 == 13
E        +  where 12.5 = calculate_total([{'desc': 'food', 'amount': 12.5}])

test_expense_tracker.py:7: AssertionError
============================= short test summary info =============================
FAILED test_expense_tracker.py::test_calculate_total_single - AssertionError: assert 12.5 == 13
=========================== 1 failed, 3 passed in 0.26s ===========================