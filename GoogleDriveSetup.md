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
    2. Make sure you choose correct account <a href="http://prntscr.com/tjh9ys" target="_blank">screenshot</a><br/>
    3. Click “Create project” button <a href="http://prntscr.com/tjhado" target="_blank">screenshot</a><br/>
    4. Enter project name and select location if needed, then press “Create” <a href="http://prntscr.com/tjhb49" target="_blank">screenshot</a><br/>
    5. Then you will be redirected to “API’s & Services” page. Click “+Enable APIs and services” button
    <a href="http://prntscr.com/tjhbzt" target="_blank">screenshot</a><br/>
    6. Choose “Google Drive API” <a href="http://prntscr.com/tjhei8" target="_blank">screenshot</a> , <a href="http://prntscr.com/tjhetx" target="_blank">screenshot</a><br/>
    7. After redirect click “create credentials” <a href="http://prntscr.com/tjhgtf" target="_blank">screenshot</a><br/>
    8. Setup as shown on screenshot <a href="http://prntscr.com/tjhhz8" target="_blank">screenshot</a><br/>
    9. Click “Set up consent screen” <a href="http://prntscr.com/tjhi6w" target="_blank">screenshot</a><br/>
    10. Select previously created project <a href="http://prntscr.com/tjhiqx" target="_blank">screenshot</a><br/>
    11. Select “External” and click “Create” <a href="http://prntscr.com/tjhj36" target="_blank">screenshot</a><br/>
    12. Enter App name and click “Save” <a href="http://prntscr.com/tjijw4" target="_blank">screenshot</a>, <a href="http://prntscr.com/tjhlp0" target="_blank">screenshot</a><br/>
    13. Click “Credentials” menu item <a href="http://prntscr.com/tjhlz2" target="_blank">screenshot</a><br/>
    14. Click “+Create credentials” and select “OAuth client ID” <a href="http://prntscr.com/tjhmg4" target="_blank">screenshot</a><br/>
    15. Select “Web application” application type and enter name. Leave section below empty for now. Click “Create”
    <a href="http://prntscr.com/tjhn1p" target="_blank">screenshot</a><br/>
    16. Note that for now there is a limit in 100 logins until app will require verification. Below you can see client
    ID and client secret. You will need them in the next steps. <a href="http://prntscr.com/tjhr3k" target="_blank">screenshot</a><br/>
    17. Next go to your salesforce org’s main setup, type “auth” in search field, select “Auth. Providers” item and
    click “New” button <a href="http://prntscr.com/tjhveq" target="_blank">screenshot</a><br/>
    18. Select “Google” provider type <a href="http://prntscr.com/tjhvrs" target="_blank">screenshot</a><br/>
    19. Enter provider name, consumer key (google client ID mentioned earlier) and consumer secret (google client
    secret). In Authorize Endpoint URL field enter following:
    <a>https://accounts.google.com/o/oauth2/auth?access_type=offline&approval_prompt=force</a> , in Token Endpoint URL enter
    <a>https://accounts.google.com/o/oauth2/accessToken</a> , in Default Scopes enter <a>openid email profile
    https://www.googleapis.com/auth/drive</a> , then click “Save” <a href="http://prntscr.com/tjhy19" target="_blank">screenshot</a><br/>
    20. Enter salesforce org’s domen URL in Authorized JavaScript origins section of a google credentials page, enter
    URL’s from Salesforce Configuration section in Authorized redirect URLs section of a google credentials page
    <a href="http://prntscr.com/tjhyfa" target="_blank">screenshot</a>, <a href="http://prntscr.com/tjhzef" target="_blank">screenshot</a><br/>
    21. Go again to your salesforce org’s main setup, type “named” in search field, select “Named Credentials” item and
    click “New Named Credential” button <a href="http://prntscr.com/tji0sk" target="_blank">screenshot</a><br/>
    22. Enter label and name, in URL field enter <b>https://www.googleapis.com</b> , select Identity Type “Per User”,
    Authorization Protocol “OAuth 2.0”, in Authentication Provider field select previously created provider, in Scope
    field enter <a>openid email profile https://www.googleapis.com/auth/drive</a> , and make sure all checkboxes selected as
    shown on screenshot <a href="http://prntscr.com/tji26u" target="_blank">screenshot</a><br/>
    23. Because of Start Authentication Flow on Save checkbox from previous step you will be redirected to google’s
    select account page and after to google’s authentication page, where you need to click “Advanced” link and then
    click on “Go to salesforce.com” link and confirm all the following steps <a href="http://prntscr.com/tji388" target="_blank">screenshot</a>,
    <a href="http://prntscr.com/tji3cp" target="_blank">screenshot</a><br/>
    24. After confirming you will be redirected back to SF page and Administration Authentication Status will be changed
    to “Authenticated as...” <a href="http://prntscr.com/tji421" target="_blank">screenshot</a><br/>
    25. Go to SF main setup, type “custom” in search field, select “Custom Metadata Types”, find “CB Google Drive
    Connect Settings” and click “Manage Records” link <a href="http://prntscr.com/tji5yx" target="_blank">screenshot</a><br/>
    26. Find “CBGDConnect” item (there is should be only one) and click “Edit” link <a href="http://prntscr.com/tji663" target="_blank">screenshot</a><br/>
    27. In Named Credential Name field enter name of previously created Named Credential, then click “Save”
    <a href="http://prntscr.com/tji6gt" target="_blank">screenshot</a><br/>
    28. Add “CB Connect” permission set to needed users <a href="http://prntscr.com/tji768" target="_blank">screenshot</a><br/>
    29. In order to login each user need to go to their settings and create new Authentication Settings for External
    Systems <a href="http://prntscr.com/tji4e4" target="_blank">screenshot</a>, <a href="http://prntscr.com/tji4ne" target="_blank">screenshot</a><br/>
    30. Set up as shown on screenshot, make sure that “Start Authentication Flow on Save” checkbox is checked, then
    click “Save”, repeat google’s authentication procedure (each user can login to a different google drive)
    <a href="http://prntscr.com/tji546" target="_blank">screenshot</a><br/>
    31. Check if Google Drive connection works: <a href="http://prntscr.com/tjj9k7" target="_blank">screenshot</a><br/>

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