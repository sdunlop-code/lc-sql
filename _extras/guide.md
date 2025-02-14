---
layout: page
title: "Instructors' Guide"
---

____
# Tips and Tricks

____
## Making a handout

Librarians like handouts. To make a handout for this lesson, adapt/print from [https://librarycarpentry.org/lc-sql/reference](https://librarycarpentry.org/lc-sql/reference).

____
# General notes of SQL

> **database** (dā'tə-bās') noun:
> "A collection of data arranged for ease and speed of search and retrieval by a computer"
>
> — The American Heritage® Science Dictionary
{: .quotation}

*   Three common options for storing data
*   Text
    *   Easy to create, work well with version control
    *   But then we have to build search and analysis tools ourselves
*   Spreadsheets
    *   Good for simple analyses
    *   But don't handle large or complex data sets well
*   Databases
    *   Include powerful tools for search and analysis
    *   Can handle large, complex data sets.

## Overall

Relational databases are not as widely used in science as in business,
but they are still a common way to store large data sets with complex structure.
Even when the data itself isn't in a database,
the metadata could be:
for example,
meteorological data might be stored in files on disk,
but data about when and where observations were made,
data ranges,
and so on could be in a database
to make it easier for scientists to find what they want to.

*   The first few sections (up to "Missing Data") usually go very quickly.
    The pace usually slows down a bit when null values are discussed
    mostly because learners have a lot of details to keep straight by this point.
    Things *really* slow down during the discussion of joins,
    but this is the key idea in the whole lesson:
    important ideas like primary keys and referential integrity
    only make sense once learners have seen how they're used in joins.
    It's worth going over things a couple of times if necessary (with lots of examples).

*   The sections on creating and modifying data,
    and programming with databases,
    can be dropped if time is short.
    Of the two,
    people seem to care most about how to add data (which only takes a few minutes to demonstrate).

*   Simple calculations are actually easier to do in a spreadsheet; the
    advantages of using a database become clear as soon as filtering
    and joins are needed.  Instructors may therefore want to show a
    spreadsheet with the information from the four database tables
    consolidated into a single sheet, and demonstrate what's needed in
    both systems to answer questions like, "What was the average
    radiation reading in 1931?"

*   Some advanced learners may have heard that NoSQL databases
    (i.e., ones that don't use the relational model)
    are the next big thing,
    and ask why we're not teaching those.
    The answers are:
    1.  Relational databases are far more widely used than NoSQL databases.
    2.  We have far more experience with relational databases than with any other kind,
        so we have a better idea of what to teach and how to teach it.
    3.  NoSQL databases are as different from each other as they are from relational databases.
        Until a leader emerges, it isn't clear *which* NoSQL database we should teach.

## Resources

*   `data/*.csv`: CSV versions of data in sample survey database.
*   `bin/create-db.sql`: generate survey database used in examples based on CSV.
