---
title: Mather Family Libraries
permalink: /docs/matherfamilylibraries/
csvlink: https://github.com/judaicadh/bibliothecahebraicaatlantica/blob/master/_data/Mather_Family_Libraries.csv
textlink: "Tuttle, J. Herbert. (1910). The libraries of the Mathers. Worcester, Mass.: Davis Press."
textview: https://hdl.handle.net/2027/hvd.32044080260326?urlappend=%3Bui=embed
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
      {% for entry in site.data.Mather_Family_Libraries %}
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
      {% endfor %}
    </tbody>
  </table>
</div>
