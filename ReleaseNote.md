<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>CloudBudget2.0 Release Note</title>
</head>

<h1 id='pageTop'>CloudBudget2.0 Summer 2020 Release Note</h1>
<div>
    <p>List of Summer 2020 additives</p>

    <ul>
        <li><a href="ReleaseNote.html#budgetApp">Budget Application</a></li>
        <li><a href="ReleaseNote.html#budgetAppSheet">Budget App Sheet</a></li>
        <li><a href="ReleaseNote.html#googleDrive">Google Drive</a></li>
        <li><a href="ReleaseNote.html#PostingRules">Posting Rules</a></li>
        <li><a href="ReleaseNote.html#CBalances">CBalances</a></li>
        <li><a href="ReleaseNote.html#additional">CB Reports</a></li>
        <li><a href="ReleaseNote.html#additional">Report Configurator</a></li>
        <li><a href="ReleaseNote.html#additional"></a>FF Integration</li>
        <li><a href="ReleaseNote.html#additional"></a>Other</li>
    </ul>
    <p>You can find additional information for each item below.</p>


    <br/>
    <h3 id='budgetApp'>Budget Application</h3>
     - Budget Application allows enter amounts into transaction lines much conveniently

    <p>The main application can have several child applications,
        each of which can have its own child items, etc.
        The structure is presented in a convenient form on the table (see screen).
        Table filters allow you to see only a list of required applications.</p>
    <img src="images/BA1.PNG" alt="App Structure" class="inline"/>

    <br/>
    <h3 id='appView'>App view</h3>
    <p>Typically, an app consists of one section (inc or exp),
        but you can also use them simultaneously</p>
    <img src="images/BA2.png" alt="App View" class="inline"/>

    <br/>
    <h3 id='topDown'>Top-down approach</h3>

    <br/>
    <h3>Bottom-up approach</h3>

    <br/>
    <h3 id='sharing'>Sharing rules</h3>

    <br/>
    <h3 id='excel'>Excel export/import</h3>
    <p>App allows you to upload data to an Excel file.
        Data in excel file can be changed. You can add or remove lines.
        It is important to keep the file format, otherwise the file cannot be imported back</p>
    <img src="images/BA3.png" alt="Export to Excel" class="inline"/>
    <p>After the data is downloaded back, you will receive a message about the successful download
        or import errors</p>
    <img src="images/BA4.png" alt="Import from Excel" class="inline"/>

    <br/>
    <h3 id='additional'>Additional Features</h3>
    <ul>
        <li>An App cannot be "Posted" until all its subsidiary apps are not "Posted"</li>
        <li>Clone</li>
        <li>Interface Permissions</li>
    </ul>

</div>
<br/>


<br/>
<hr/>
<div>
    Navigate to:
    <p><a href="https://cloudbudgetinc.github.io/Docs/CBCore">CB Base Documentation</a></p>
    <p><a href="https://cloudbudgetinc.github.io/Docs/BudgetTemplate">Budget App Template</a></p>
</div>

<button onclick="topFunction()" id="myBtn" title="Go to top">Top</button>

<script>
    let mybutton = document.getElementById("myBtn");
    window.onscroll = function () {
        scrollFunction()
    };

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