---
title: Massachusettes Historical Society
permalink: /docs/mhs/
csvlink: https://github.com/judaicadh/bibliohebraicaatlantica/blob/master/Massachusettes%20Historical%20Society/WorldCat_3752085.csv
textlink: "Massachusetts Historical Society. Library., . (1796). Catalogue of books in the Massachusetts Historical Society library. Boston: Printed by S. Hall, no. 53, Cornhill.
"
textview: "https://hdl.handle.net/2027/nyp.33433069263154?urlappend=%3Bui=embed"
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
        {% if entry.Library == "Massachusetts Historical Society"%}
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
