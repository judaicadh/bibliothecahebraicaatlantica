---
title: William Byrd
permalink: /docs/williambyrd/
csvlink: https://github.com/judaicadh/bibliohebraicaatlantica/blob/master/William%20Byrd/WorldCat_3742311.csv
textlink: "Hayes, K. J. (1997). The library of William Byrd of Westover. Madison, Wis.: Madison House."
textview: https://hdl.handle.net/2027/pur1.32754004402792?urlappend=%3Bui=embed
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
        {% if entry.Library == "William Byrd"%}
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

<img src="http://t2.gstatic.com/images?q=tbn:ANd9GcTrfwmEQ3_NjYo27GT6vWNrdePrXzDYAfgfUIa-G04r5eDQt4dm" width="200" align="middle">
