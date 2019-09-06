---
title: Benjamin Franklin
permalink: /docs/benjaminfranklin/
csvlink: "https://github.com/judaicadh/bibliothecahebraicaatlantica//blob/master/Benjamin%20Franklin/WorldCat_3743313.csv"
textlink: "Wolf, Edwin, and Kevin J. Hayes. 2006. The library of Benjamin Franklin. Philadelphia: American Philosophical Society/Library Co. of Philadelphia."
---

<div class="row">
  <table id="library-table" class="row-border" cellspacing="0" width="100%">
    <thead>
        <tr>
          <th>OCLC #</th>
          <th>Title</th>
          <th>Author</th>
          <th>Language</th>
          <th>Item type</th>
          <th>Publication</th>
          <th>Publisher</th>
          <th>Database</th>
          <th>Notes</th>
          <th>Added date</th>
          <th>Library</th>
        </tr>
    </thead>

    <tbody>  
      {% for entry in site.data.summary %}
        {% if entry.Library == "Benjamin Franklin"%}
          <tr>
            <td>{{entry.OCLC}}</td>
            <td>{{entry.Title}}</td>
            <td>{{entry.Author}}</td>
            <td>{{entry.Language}}</td>
            <td>{{entry.Item_type}}</td>
            <td>{{entry.Publication}}</td>
            <td>{{entry.Publisher}}</td>
            <td>{{entry.Database}}</td>
            <td>{{entry.Notes}}</td>
            <td>{{entry.Date_Added}}</td>
            <td>{{entry.Library}}</td>
          </tr>
        {% endif %}
      {% endfor %}
    </tbody>
  </table>
</div>

---------/

<iframe frameborder="0" scrolling="no" style="border:0px" src="https://books.google.com/books?id=ibgiSlbMDPUC&lpg=PP1&pg=PP1&output=embed" width="500" height="500"></iframe>
