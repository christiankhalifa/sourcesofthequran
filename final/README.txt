The Intertextual Qur’an Project
===============================
200 Years of Collated Sources

A scholarly synopsis that places each Qur'anic narrative focus point beside its
extra-biblical Jewish and Christian antecedents and the biblical counter-traditions
recorded for it — three columns, read side by side. Qur'anic text follows the
Maulana Wahiduddin Khan (MWK) English translation.

Files in this folder
--------------------
  index.html                 The website (open or serve this).
  IQP_Database__Sharu_.xlsx  The database. This is the file you edit to add data.
  quran-data.js              The MWK translation, used to display verse text.
  xlsx.full.min.js           The spreadsheet reader (SheetJS).

Keep all four files together in the same folder.

How to run it (recommended)
---------------------------
So the page can read the spreadsheet automatically, serve the folder:

  1. Open a terminal in this folder.
  2. Run:   python3 -m http.server 8000
  3. Open:  http://localhost:8000/

Adding or changing antecedents
------------------------------
  1. Edit IQP_Database__Sharu_.xlsx and save it (keep the same filename and the
     same column headers — the page matches columns by header name, so columns
     may be reordered but should keep their names).
  2. In the browser, press "Reload data" (or just refresh the page).
     New rows appear immediately. Empty fields are never shown.

The three sheets
----------------
  Biblical               -> the third column (biblical references).
  Extra-Biblical Jewish  -> blue antecedent cards in the middle column.
  Extra-Biblical Christian -> plum antecedent cards in the middle column.

Rows are joined by Broad Topic + Focus Point. Subtopic is used for grouping in
the "By Topic" view.

Opening without a server
------------------------
You can also just double-click index.html. The database is already built into
the page, so everything loads straight away (the status shows "Built-in").

Note: the built-in copy is a snapshot. Edits you make to the .xlsx are picked up
automatically only when the folder is served (see above; status shows "Live").
When opened by double-click, press "Reload data" and choose the edited .xlsx to
view your changes, or ask for the built-in copy to be refreshed.
