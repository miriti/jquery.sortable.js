jquery.sortable.js
==================

Html table sorting plugin for jQuery

Usage
-----
Include jquery.sortable.js to your html page:
```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script src="js/jquery.sortable.js"></script>
```

Update your table markup:
```html
<table class="sortable">
  <thead data-head="true">
    <tr>
      <th data-sort-column="true">ID</th> <!-- this column will be sortable -->
      <th data-sort-column="true">Name</th> <!-- this column will be sortable -->
      <th data-sort-column="true">Last name</th> <!-- this column will be sortable -->
      <th data-sort-column="true">Birthday</th> <!-- this column will be sortable -->
      <th>Additional info</th> <!-- this column will *NOT* be sortable -->
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>John</td>
      <td>Doe</td>
      <td data-sort-value="1987-12-08">December 8, 1987</td>
      <!--
      'data-sort-value' determines value to be used in comparison while sorting.
      Comparison of numbers is much faster then strings so converting strings to 
      numbers (when it is possible) will increase performance. For example you can
      use '565920000' instead of '1987-12-08'.
      -->
      <td>Foo bar</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Jane</td>
      <td>Doe</td>
      <td data-sort-value="1992-08-15">August 15, 1992</td>
      <td>Foo</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Phillip</td>
      <td>Burns</td>
      <td data-sort-value="1965-05-03">May 3, 1965</td>
      <td>Bar</td>
    </tr>
  </tbody>
</table>
```
