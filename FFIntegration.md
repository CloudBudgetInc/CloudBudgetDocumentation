<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>FF Integration</title>
</head>

<h1 id='pageTop'>FF Integration</h1>
<div>
    <p>FF Integration allows to import FF Reporting Balances to CloudBudget side using specific congifuration of the
        mapping.
    </p>

    <ul>
        <li><a href="FFIntegration.html#config">Setup a Configuration</a></li>
        <li><a href="FFIntegration.html#run">Run Import</a></li>
        <li><a href="FFIntegration.html#features">Features</a></li>
    </ul>

    <p>You can find additional information for each item below.</p>


    <br/>
    <h3 id='config'>Setup a Configuration</h3>

    <p>Text</p>
    <img src="images/FFI1.png" alt="FF Integration Interface" class="inline"/>

    <br/>
    <h3 id='run'>Run Import</h3>
    <p>Text</p>


    <br/>
    <h3 id='features'>Features</h3>
    <p>The integration algorithm is as follows:</p>
    <p>1. Batch deletes previous imported records based on selected dates and the mapping configuration</p>
    <p>2. The controller checks whether all the necessary analysts are present on the CloudBudget side (Accounts,
        Dimensions, Locations, etc)</p>
    <p>3. Batch creates a list of new Records of CB Reporting Balances, based on FF Reporting Balances,
        selected dates and the current configuration settings</p>

    <br/>


    <br/>
    <hr/>
    <div>
        Navigate to:
        <p><a href="https://fallentol.github.io/CloudBudget/CB2/CBCore">CB Base Documentation</a></p>
    </div>

    <button onclick="topFunction()" id="myBtn" title="Go to top">Top</button>

    <script>
        var mybutton = document.getElementById("myBtn");
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