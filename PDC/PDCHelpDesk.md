<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>PDC Helpdesk</title>
</head>

<h2 id='pageTop'>PDC Helpdesk</h2>
<hr/>
<br/>
<br/>

<div>
    <p>A list of guide links for PDC users</p>
    <br/>
    <ul>
        <li><p><a href="https://cloudbudgetinc.github.io/Documentation/PDC/AddingGLAccountGuide">Adding GL Accounts Guide</a></p></li>
        <li><p><a href="https://cloudbudgetinc.github.io/Documentation/GoogleDriveSetup">Google Drive Setup</a></p></li>
    </ul>
</div>
<br/>

<br/>
<hr/>


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