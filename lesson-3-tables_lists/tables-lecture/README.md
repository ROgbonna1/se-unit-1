# Unit 1 Lesson 3 - Tables
## Code-a-long Guide

1. Adjust width and height of rows and columns.
  ```css
  col {
    width: 100px;
  }

  tr {
    height: 100px;
  }
  ```

2. Add and collapse borders by targeting table and all of it's descendants.
  ```css
    table, table * {
    border: 1px solid black;
    border-collapse: collapse;
  }
  ```

3. Play around with text alignment by targeting the `text-align` property of the `td` element.
  ```css
    td {
    text-align: center;
  }
  ```

4. Add `scope` attributes to `<th>`s and then target those attributes for styling using an attribute selector.
  ```css
    th[scope="row"] {
    background-color: #0b0775;
    color: #ffffff;
  }
  ```
5. Add `<colgroup>` elements and demonstrate how that facilitates styling targeted at table _columns_.
  ```html
   <colgroup>
      <col>
      <col>
      <col>
      <col>
      <col>
      <col>
      <col>
      <col>
    </colgroup>
  ```

6. Add an ID to a `<col>` and target it for styling that way.

7. Use the `:nth-child` **pseudo-class** to target another column.
  ```css
    col:nth-child(3) {
    background-color: #e9e9e9;
    width: 200px;
  }
  ```

8. Mark up the table with `<thead>`, `<tbody>`, `<tfoot>`. Talk over the accessibility benefits.

9. Add a footer so that we can use the `colspan` attribute.
  ```html
   <tfoot>
      <tr>
        <td colspan="8">This is the footer</td>
      </tr>
   </tfoot>
  ```

10. Target the `<tfoot>` element to give the footer a common background color.
  ```css
  tfoot {
    background-color: #e9e9e9;
  }
  ```

11. Demonstrate how we can great grouped headers by deleting the "4th period" cell and setting the "3rd period" `rowspan` attribute to `"2"`.
  ```html
  <th rowspan="2" scope="row">3rd Period</th>
  ```


