---
title: John Adams
permalink: /docs/johnadams/
csvlink: https://github.com/judaicadh/bibliothecahebraicaatlantica/blob/master/_data/John_Adams.csv
textlink:  "<br /> Adams, J. Quincy. (1938). A catalogue of the books of John Quincy Adams: deposited in the Boston athenæum, with notes on books, Adams seals and book-plates. Boston: Athenæum. <br /> Metcalf, E. Wight., Adams, J., Boston Public Library. Adams Collection., . (1823). Deeds and other documents relating to the several pieces of land, and to the library presented to the town of Quincy by President Adams ; together with a catalogue of the books. Cambridge [Mass.]: Printed by Hilliard and Metcalf."
textview: https://hdl.handle.net/2027/nyp.33433081827895?urlappend=%3Bui=embed
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
      {% for entry in site.data.John_Adams %}
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
