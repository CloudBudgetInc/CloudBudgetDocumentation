<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>Budget App</title>
</head>

<style>
    .exNAme {
        color: red;
        font-weight: bold;
    }
    table, th, td {
  		border: 1px solid #111;
  		border-collapse: collapse;
  		padding: 2px;
	}
</style>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.0/jquery.min.js"></script>
<h1>Dimensions</h1>
<div>
To configure view of the Primary Document go to its Dimension.<br/>
To customize view of the Primary Document, set up next fields:<br/>
1. Name - The name of Primary Document:<br/>
2. Page Header - The public name of Primary Document that will be displayed on the view page, in the list view etc.;<br/>
3. Order Number - ? ;<br/>
4. Access - Tags of sharing user groups;<br/>
5. Approval Process - Aproval Process for Primary Document;<br/>
6. Functional Component Name - API Name of the custom component that will be used on the Primary Document View;<br/>
13. Related Dimension - Choose related to the Primary Document items, for displaying in related lists on the view page;<br/>
14. Custom Mode - If "false", work as standart list view. If "true", group items by Periods;<br/>
15. First Group Field - Choose field to group related items in Custom Mode;<br/>
16. Period Field - Choose field of the related item in wich Period is stored;<br/>
17. Value Field - Choose amount field, that will be shown in the Custom Mode view;<br/>
<img src="images/Dim1.png" alt="Creating of the Primary Dimension">
<br/>
To customize UI of the Primary Document there are 6 fields.<br/>
Logicaly view page consist of three blocks: "Header", "Body", "Footer".<br/>
<table width="300px">
	<tbody>
		<tr style="border: 2px solid white;"><td align="center">Header</td></tr>
		<tr style="border: 2px solid white;"><td align="center">Body</td></tr>
		<tr style="border: 2px solid white;"><td align="center">Footer</td></tr>
	</tbody>
</table>
Each block has 1 - 3 columns.<br/>
<table border="1" width="400px">
	<tbody>
		<tr><td colspan="3" style="border: 2px solid white;" align="center">Header Width = 1</td></tr>
		<tr>
			<td colspan="3" style="border: 2px solid white;" align="center">
				<div style="display: flex;">
				<div style="width: 49%;border-right: 2px solid white;">Body Width = 2</div>
				<div style="width: 49%;">Body Width = 2</div>
				</div>
			</td>			
		</tr>
		<tr>
			<td style="border: 2px solid white;" align="center">
				<div style="display: flex;">
					<div style="width: 33%;border-right: 2px solid white;">Footer Width = 3</div>
					<div style="width: 33%;border-right: 2px solid white;">Footer Width = 3</div>
					<div style="width: 33%;">Footer Width = 3</div>
				</div>
			</td>
		</tr>
	</tbody>
</table>
7. Header Height - number of fields in the header columns;<br/>
8. Header Width - number of columns in the header block (1-3);<br/>
9. Body Height - number of fields in the body columns;<br/>
10. Body Width - nember of columns in the body block (1-3);<br/>
11. Footer Height - number of fields in the footer columns;<br/>
12. Footer Width - nember of columns in the footer block (1-3);<br/>
<img src="images/Dim2.png" alt="Creating of the Primary Dimension">
<br/>
Each field has its own settings:<br/>
18. Visible - If "true" field will be displayed on the view page;<br/>
19. Title field - Name that will be used as label for concrete field on the view page;<br/>
20. Edit - Where this field must be shown. "Card" - table and card; "Table" - only table;<br/>
21. Access - User or group that have access to the field;<br/>
22. Block - Block where to show this field (Header, Body, Footer);<br/>
23. Column - Column where to show this field (1 - 3);<br/>
24. Order - Order Number, position where to show this field inside the column (vertical align);<br/>
<img src="images/Dim3.png" alt="Creating of the Primary Dimension">

<br/>
<h4>Exception description:</h4>
<table style="width: 100%">
	<tr>
		<th>Exception</th>
		<th>Description</th>
	</tr>
	<tr>
		<td><span class="exName">EXCEPTION: </span></td>
		<td> </td>
	</tr>
</table>

<br/>
<hr/>
<div>
    Navigate to:
   <p></p><p><a href="https://cloudbudgetinc.github.io/Docs/CBCore">Main Page</a></p><p></p>
</div>

<button onclick="topFunction()" id="myBtn" title="Go to top">Top</button>

<script>
var mybutton = document.getElementById("myBtn");
window.onscroll = function() {scrollFunction()};
function scrollFunction() {
    mybutton.style.display = document.body.scrollTop > 20 || document.documentElement.scrollTop > 20 ? "block" : "none";
}
function topFunction() {
  document.body.scrollTop = 0;
  document.documentElement.scrollTop = 0;
}
</script>

<style>
#myBtn {
  display: none;
  position: fixed;
  bottom: 20px;
  right: 30px;
  z-index: 99;
  font-size: 18px;
  border: 1px solid #b5e853;
  outline: none;
  background-color: #171717;
  color: #b5e853;
  cursor: pointer;
  padding: 15px;
  border-radius: 4px;
}

#myBtn:hover {
  background-color: #181818;
}
</style>

</body>
</html>
