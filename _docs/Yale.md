---
title: Yale
permalink: /docs/yale/
csvlink: https://github.com/judaicadh/bibliohebraicaatlantica/tree/master/Yale
textlink: "Yale University. Library., . (1808). Catalogue of books in the library of Yale-College, New-Haven, January, 1808. New-Haven: Printed by Oliver Steele & Co.."
textview: https://hdl.handle.net/2027/nnc1.50169434?urlappend=%3Bui=embed
---

<div class="row">
  <table id="library-table" class="display" cellspacing="0" width="100%">
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
        {% if entry.Library == "Yale"%}
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
