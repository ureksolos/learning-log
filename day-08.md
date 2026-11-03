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
Enter Book Title: Lord of the mysteries
Enter Author ID: 101
Enter Year: 2018
Enter Author's name: Cuttlefish that loves diving

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 1
Enter Book Title: Shura's Wrath
Enter Author ID: 121
Enter Year: 2012
Enter Author's name: Mars Gravity

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 5
PS C:\Users\succe\Documents\python-practice> python 13_books.py

--- Books Menu ---
1) Add book
2) List all books (with author name)
3) Find book by author
4) Delete book
5) Quit
Choose an option (1-5): 2
Lord of the mysteries — Cuttlefish that loves diving (2018)
Shura's Wrath — Mars Gravity (2012)

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