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

Update your table markup.
1. Add `data-header` attribute equals `true` to the `<thead>` of your table
2. Add `data-sort-column` attribute equals `true` to every column header that should be sortable
3. Add `data-body` attribute equals `true` to `<tbody>` of your table
```html
<table class="sortable" border="1">
    <thead data-header="true">
        <tr>
            <th data-sort-column="true">ID</th>
            <th data-sort-column="true">Name</th>
            <th data-sort-column="true">Last Name</th>
            <th data-sort-column="true">Birthday</th>
            <th>Note</th>
        </tr>
    </thead>
    <tbody data-body="true">
        <tr>
            <td>1</td>
            <td>John</td>
            <td>Doe</td>
            <td data-sort-value="1987-12-08">December 8, 1987</td>
            <td>Morbi id felis metus</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Jane</td>
            <td>Pope</td>
            <td data-sort-value="1975-10-14">October 14, 1975</td>
            <td>Maecenas id enim vel lectus lobortis molestie</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Bob</td>
            <td>Ludwig</td>
            <td data-sort-value="1995-05-05">May 5, 1995</td>
            <td>Cras mi purus, dapibus in ipsum a, malesuada facilisis dolor</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Anne</td>
            <td>Heisenberg</td>
            <td data-sort-value="1967-01-31">January 31, 1967</td>
            <td>Aliquam egestas tincidunt purus, a sagittis neque lacinia vehicula</td>
        </tr>
        <tr>
            <td>5</td>
            <td>Kate</td>
            <td>Miller</td>
            <td data-sort-value="1991-08-17">August 17, 1991</td>
            <td>Pellentesque vitae nulla elit</td>
        </tr>
    </tbody>
</table>
```

Call to jQuery.tablesorter whenevery DOM will be ready:

```html
<script>
    $(function() {
        $('.sortable').sortable();
    });
</script>
```
