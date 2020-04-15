---
title: Jonathan Edwards
permalink: /docs/jonathanedwards/
csvlink: https://github.com/judaicadh/bibliothecahebraicaatlantica/blob/master/_data/Jonathan_Edwards.csv
textlink: "http://library.princeton.edu/libraries/firestone/rbsc/aids/1920_Edwards_Collection.pdf"
textview: http://library.princeton.edu/libraries/firestone/rbsc/aids/1920_Edwards_Collection.pdf
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
      {% for entry in site.data.Jonathan_Edwards %}
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
