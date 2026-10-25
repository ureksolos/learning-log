# Day 2

- Date: 2026-10-25
- Hours planned: 6
- Hours achieved: 5
- What i built: 01_basics.py, 02_calculator.py, both located in python-practice repo.
- 02_tip_calculator.py:

    bill = float(input("Enter Bill: ")) # reads user input for bill
    tip_percent = float(input("Enter tip %: ")) # reads user input for tip (%)
    people = int (input("Enter number of persons: ")) reads user input for number of persons

    tip = bill * (tip_percent / 100) # calculates the tip amount using the percentage
    total = bill + tip # calculates total amount
    per_person = total / people # calculates price per person

    print (f"Tip: ${tip:.2f}") # prints tip to 2 d.p, using f strings
    print (f"Total: ${total:.2f}") # same with total
    print (f"Per-person: ${per_person:.2f}") # price per person too


- Test output for 02_calculator.py: 

    Enter Bill: 100
    Enter tip %: 15
    Enter number of persons: 3
    Tip: $15.00
    Total: $115.00
    Per-person: $38.33

- main.txt output:
    Hello, my name is Urek
    Today is 2026-10-25

- 1/0 output:
    line 1 ran
    line 2 ran
    Traceback (most recent call last):
        File "C:\Users\succe\Documents\py4e\testProgram.py", line 3, in <module>
            x = 1 / 0
                ~~^~~
    ZeroDivisionError: division by zero


- What I didn't understand: Rebuilt from memory cleanly in 6 minutes; no stalls.
- Guided resource: Watched videos on py4e.com, Completed lessons 1-3. Spent roughly 2 hours on it
- A.I Log(s): No A.I usage
- Rewritten all codes from memory


## Day 2 Acceptance Criteria Verification

| # | Acceptance Criterion | Status | Evidence |
|---|---------------------|:------:|----------|
| 1 | schedule.md public with all four windows and both tripwires | ✅ | https://github.com/ureksolos/learning-log/blob/main/schedule.md |
| 2 |  main.txt and 1/0 outputs pasted | ✅ | above |
| 3 | 02_tip_calculator.py passes the 100/15/3 → 15.00 / 115.00 / 38.33 test | ✅ | output is above |