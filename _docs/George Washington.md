---
title: George Washington
permalink: /docs/georgewashington/
csvlink: https://github.com/judaicadh/bibliohebraicaatlantica/blob/master/George%20Washington/WorldCat_3743601.csv
textlink: "Washington, G. (1890). Catalogue ..: collection of the effects of General George Washington and of his executor and nephew, Lawrence Lewis, and grand-nephew, Lorenzo Lewis ... [Philadelphia: The Bicking press."
textview: "https://hdl.handle.net/2027/nyp.33433000152250?urlappend=%3Bui=embed"
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
        {% if entry.Library == "George Washington"%}
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
