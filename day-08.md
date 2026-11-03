# Day 8
---
- **Date:** 2026-11-03
- **Hours Planned:** 6
- **Hours Achieved:** 6 (sure i spent 8+ hrs cummulatively)
- **AI Log:** No AI, just lookups on youtube, sqlbolt.com
- **Rebuild result:** Clean in 1+ hr
- **"The part I'd have to look up tomorrow is:** More practice on sqlite projects
---

## OUTPUTS

### OUTPUT 1: RESTART TEST

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 1
Enter Book Title: Brain
Enter Year: asdf
Non-numeric year detected!
Enter Author's name: Tim Cook

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 1
Enter Book Title: Renegade Immortal
Enter Year: 2009
Enter Author's name: Er Gen

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 5
PS C:\Users\succe\Documents\python-practice> python books_13.py

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 2
Brain — Tim Cook
Renegade Immortal — Er Gen (2009)

### OUTPUT 2: FIND BY AUTHOR (1 BOOK)

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 3
Enter Author Name: Mars Gravity
Shura's Wrath — Mars Gravity (2012)

### OUTPUT 3: FIND BY AUTHOR (0 BOOKS)

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 3
Enter Author Name: Masashi Kishomoto
Book not found!

### OUTPUT 4: DELETE-MISS

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 4
Enter Book Title: Shura's Wrath
Deleted 1 book

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 4
Enter Book Title: Shura's Wrath
No book found

### OUTPUT 5: EMPTY LIST

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 2
No books yet

### OUTPUT 6: Non-Numeric on Add

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 1
Enter Book Title: Renegade Immortal
Enter Author ID: 234
Enter Year: two-thousand-and-nine
Non-numeric year detected!
Enter Author's name: Er Gen        

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 2
Lord of the mysteries — Cuttlefish that loves diving (2018)
Renegade Immortal — Er Gen

### OUTPUT 7: test_format_book.py pytest output

==================================================================== test session starts ====================================================================
platform win32 -- Python 3.15.1, pytest-9.2.0, pluggy-1.7.0
rootdir: C:\Users\succe\Documents\python-practice
collected 2 items                                                                                                                                            

test_format_book.py ..                                                                                                                                 [100%]

===================================================================== 2 passed in 0.18s =====================================================================

### test_format_book.py Code:

from books_13 import format_book

def test_format_book_no_year():
    assert format_book("Brain", "Tim Cook", None) == "Brain — Tim Cook"

def test_format_book_with_year():
    assert format_book("Brain", "Tim Cook", 2024) == "Brain — Tim Cook (2024)"