<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>CloudBudget2.0 Google Drive Setup</title>
</head>

<h1 id='pageTop'>CloudBudget2.0 Google Drive Setup</h1>
<div>
    <br/>
    <p>To setup the Google Drive connection with CloudBudget do the following</p>
    <hr/>

    1. Go to <a href="https://console.developers.google.com/"> Google Console</a><br/>
    2. Make sure you choose the correct account <a href="http://prntscr.com/tjh9ys" target="_blank">(screenshot)</a><br/>
    3. Click the “Create project” button <a href="http://prntscr.com/tjhado" target="_blank">(screenshot)</a><br/>
    4. Enter the project name and select the location if needed, then press “Create” <a href="http://prntscr.com/tjhb49" target="_blank">(screenshot)</a><br/>
    5. You will be redirected to the “API’s & Services” page. Click the “+Enable APIs and services” button
    <a href="http://prntscr.com/tjhbzt" target="_blank">(screenshot)</a><br/>
    6. Choose “Google Drive API” <a href="http://prntscr.com/tjhei8" target="_blank">(screenshot)</a> , <a href="http://prntscr.com/tjhetx" target="_blank">(screenshot)</a><br/>
    7. After the redirect click “create credentials” <a href="http://prntscr.com/tjhgtf" target="_blank">(screenshot)</a><br/>
    8. Setup as shown on this screenshot <a href="http://prntscr.com/tjhhz8" target="_blank">(screenshot)</a><br/>
    9. Click “Set up consent screen” <a href="http://prntscr.com/tjhi6w" target="_blank">(screenshot)</a><br/>
    10. Select the previously created project <a href="http://prntscr.com/tjhiqx" target="_blank">(screenshot)</a><br/>
    11. Select “External” and click “Create” <a href="http://prntscr.com/tjhj36" target="_blank">(screenshot)</a><br/>
    12. Enter the appname and click “Save” <a href="http://prntscr.com/tjijw4" target="_blank">(screenshot)</a>, <a href="http://prntscr.com/tjhlp0" target="_blank">(screenshot)</a><br/>
    13. Click the “Credentials” menu item <a href="http://prntscr.com/tjhlz2" target="_blank">(screenshot)</a><br/>
    14. Click “+Create credentials” and select “OAuth client ID” <a href="http://prntscr.com/tjhmg4" target="_blank">(screenshot)</a><br/>
    15. Select the  “Web application” application type and enter the name. Leave the section below empty for now. Click “Create”
    <a href="http://prntscr.com/tjhn1p" target="_blank">(screenshot)</a><br/>
    16. Note: At this point it is possible that you will see a system message in the dialog box stating that there is a
    limit of 100 logins while the app requires Google verification (confirmation). Below you can see the Client ID and
    Client Secret. You will need these for the next steps <a href="http://prntscr.com/tjhr3k" target="_blank">(screenshot)</a><br/>
    17. Next, go to your salesforce org’s main setup, type “auth” in the search field, select “Auth. Providers” and
    click the “New” button <a href="http://prntscr.com/tjhveq" target="_blank">(screenshot)</a><br/>
    18. Select the “Google” provider type <a href="http://prntscr.com/tjhvrs" target="_blank">(screenshot)</a><br/>
    19. Enter provider name, consumer key (google client ID mentioned earlier) and consumer secret (google client
    secret).<br/>
    <ul>
        <li>In the “Authorize Endpoint URL” field enter the following URL:
            <a>https://accounts.google.com/o/oauth2/auth?access_type=offline&approval_prompt=force</a></li>
        <li>In the “Token Endpoint URL” enter: <a>https://accounts.google.com/o/oauth2/accessToken</a></li>
        <li>In “Default Scopes” enter: <a>openid email profile https://www.googleapis.com/auth/drive</a></li>
        <li>Click “Save” <a href="http://prntscr.com/tjhy19" target="_blank">(screenshot)</a></li>
    </ul><br/>
    20.Completing the URL Sections:<br/>
    <ul>
        <li>Enter the salesforce org domain URL in the “Authorized JavaScript origins” section of the google credentials page</li>
        <li>Enter the URLs from the “Salesforce Configuration” section in the “Authorized redirect URLs” section of the
            google credentials page <a href="http://prntscr.com/tjhyfa" target="_blank">(screenshot)</a>,
            <a href="http://prntscr.com/tjhzef" target="_blank">(screenshot)</a></li>
    </ul><br/>
    21. Open your salesforce org main setup, type “named” in the search field, select “Named Credentials” and then
    click “New Named Credential” <a href="http://prntscr.com/tji0sk" target="_blank">(screenshot)</a><br/>
    22. Fill in the following fields:<br/>
    <ul>
        <li>Enter any label and any name and then enter <b>https://www.googleapis.com</b> in the URL field</li>
        <li>Next, select “Identity Type” - “Per User”</li>
        <li>“Authorization Protocol” - “OAuth 2.0”</li>
        <li>in “Authentication Provider” field select the previously created provider</li>
        <li>In the “Scope” field enter "<a>openid email profile https://www.googleapis.com/auth/drive</a>"</li>
        <li>Make sure all checkboxes are selected as shown on the following screenshot
            <a href="http://prntscr.com/tji26u" target="_blank">(screenshot)</a></li>
    </ul><br/>
    23. As the “Start Authentication Flow on Save” checkbox was selected in the previous step you will be:<br/>
    <ul>
        <li>Redirected to a Google’s authorization page where you will select the account.</li>
        <li>Next you will be sent to Google’s authentication page, where you need to click the “Advanced” link and then
            click the “Go to salesforce.com” link and confirm all the following steps
            <a href="http://prntscr.com/tji388" target="_blank">(screenshot)</a>,
            <a href="http://prntscr.com/tji3cp" target="_blank">(screenshot)</a></li>
    </ul><br/>
    24. After confirming you will be redirected back to the Salesforce page and the “Administration Authentication
    Status” will be changed to “Authenticated as...” <a href="http://prntscr.com/tji421" target="_blank">(screenshot)</a><br/>
    25. Go to the Salesforce main setup, type “custom” in the search field, select “Custom Metadata Types,” find “CB Google
    Drive Connect Settings,” and click the “Manage Records” link <a href="http://prntscr.com/tji5yx" target="_blank">(screenshot)</a><br/>
    26. Find “CBGDConnect” item (there should be only one) and click the “Edit” link <a href="http://prntscr.com/tji663" target="_blank">(screenshot)</a><br/>
    27. In the “Named Credential Name” field enter the name of the “Named Credential” (object) as created in step 22. Note: Do not use the name found in the “Label” field.
    <a href="http://prntscr.com/tlfjtv" target="_blank">(screenshot)</a> Click “Save” <a href="http://prntscr.com/tji6gt" target="_blank">(screenshot)</a><br/>
    28. Create new permission set:<br/>
    <ul>
        <li>Open your salesforce org main setup, type “permission” in the search field, select “Permission Sets” and then click “New”
            <a href="http://prntscr.com/tluqa8" target="_blank">(screenshot)</a></li>
        <li>Enter any name and any label, click “Save” <a href="http://prntscr.com/tlurk9" target="_blank">(screenshot)</a></li>
        <li>Type “named” in the search field of this new permission set and select “Named Credentials Access” <a href="http://prntscr.com/tlusab" target="_blank">(screenshot)</a></li>
        <li>Click “Edit” <a href="http://prntscr.com/tlutgm" target="_blank">(screenshot)</a></li>
        <li>Click on the checkbox near to the previously created named credential and click “Save” <a href="http://prntscr.com/tlvurm" target="_blank">(screenshot)</a></li>
        <li>Type “metadata” in the search field and select “Custom Metadata Types” <a href="http://prntscr.com/tlw44e" target="_blank">(screenshot)</a></li>
        <li>Click “Edit” <a href="http://prntscr.com/tlw44e" target="_blank">(screenshot)</a></li>
        <li>Click on the checkbox near to the “CB Google Drive Connect Setting” and click “Save” <a href="http://prntscr.com/tlw594" target="_blank">(screenshot)</a></li>
        <li>Add this permission set for all users <a href="http://prntscr.com/tlwg77" target="_blank">(screenshot)</a></li>
    </ul><br/>
    29. In order to login each user need to go to their settings and create new Authentication Settings for External Systems
    <a href="http://prntscr.com/tji4e4" target="_blank">(screenshot)</a>, <a href="http://prntscr.com/tji4ne" target="_blank">(screenshot)</a><br/>
    30. Set up as shown on screenshot, make sure that “Start Authentication Flow on Save” checkbox is checked, then
    click “Save”, repeat google’s authentication procedure (each user can login to a different google drive)
    <a href="http://prntscr.com/tji546" target="_blank">(screenshot)</a><br/>
    31. Check if Google Drive connection works: <a href="http://prntscr.com/tjj9k7" target="_blank">(screenshot)</a><br/>

</div>
<br/>

<br/>
<hr/>
<!--<div>
    Navigate to:
    <p><a href="https://cloudbudgetinc.github.io/Docs/CBCore">CB Base Documentation</a></p>
</div>-->

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