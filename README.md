# publications-list
Database driven Publication Lists for multiple Related Researchers and/or Departments

The Problem: Publication lists of many Professors/Researchers are out of date.

One Solution: Centrally updated/maintained database of publications that can also be updated by researchers.  
https://advance.science.sfu.ca/biology/publications/search.php?search=eelle
https://advance.science.sfu.ca/bpk/publications/search.php?search=ablaber

Features:
Database on FileMaker Server;  (could be modified for MySQL)
Easily updatable by staff using Filemaker Client
Researchers can add new publications and edit their own existing publications via web interface
Researchers/staff can designate others to edit their publications
Publications linked to Researchers/ Faculty by unique identifier (computingID) 
Publication Lists display in different formats for different disciplines
Configuration/customization in a single file 
Displays name of researcher and links to researcher's home page
Customized for each dept, and/or for individual researchers
e.g, Chemistry uses ACS format except one prof prefers APA format
 
Page wording and links appropriate based on number of publications returned
Currently has two formats, one ACS (Chemistry), the other APA (General Science). 
More formats can be added with minimal effort.
Selected Publications
Author + Keyword Search
 
Keyword Search
 
iframe (embedded within another page- scroll down a bit to see publications)

Constraints:
I only add publications from the Web of Science
One field for authors (can't customize the format of the authors)
One database record per publication means common authors share the record.
 
Selected Publications are selected for all co-authors
 
Department should have common format for link to researcher's home page, 
e.g. dept/people/computingid.html (if not, link to the common Faculty page as for Statistics or use the configuration setup page)
Multiple-Authored Publications as found in Medical & high-energy Physics research are a problem 
for linking authors, indexing, and displaying of publications.  I have a calculation where if there are more than 30 authors I change it to 20 authors et al. (used in physics but might need it for for all)
search.php (which returns all found and allows instant searches) is too slow for researchers with >500 publications. I have a different search page for this but I don't think they will be interested anyway
 

Work Involved:
Publications must be downloaded/uploaded and then linked to researchers- this is partially automated but it helps to have knowledge of the researchers.

Future:
 
HTML Markup (e.g. italicized species names, live links)- easy, just need to test
Serve with MySQL database rather than FileMaker. I previously recoded it and 
served from a MySQL database using Bibliograph https://github.com/cboulanger/bibliograph
 
Would like to recode it for MySQL and bibutils https://sourceforge.net/projects/bibutils/
and wikindx or refbase http://www.refbase.net/index.php/Table_refs

