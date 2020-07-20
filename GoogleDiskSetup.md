<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>CloudBudget2.0 Google Disk Setup</title>
</head>

<h1 id='pageTop'>CloudBudget2.0 Google Disk Setup</h1>
<div>
    <p>List of Summer 2020 additives</p>

    1. Go to https://console.developers.google.com/
    2. make sure you choose correct account http://prntscr.com/tjh9ys
    3. click “Create project” button http://prntscr.com/tjhado
    4. Enter project name and select location if needed, then press “Create” http://prntscr.com/tjhb49
    5. Then you will be redirected to “API’s & Services” page. Click “+Enable APIs and services” button http://prntscr.com/tjhbzt
    6. Choose “Google Drive API” http://prntscr.com/tjhei8 ,  http://prntscr.com/tjhetx
    7. After redirect click “create credentials” http://prntscr.com/tjhgtf
    8. Setup as shown on screenshot http://prntscr.com/tjhhz8
    9. Click “Set up consent screen” http://prntscr.com/tjhi6w
    10. Select previously created project http://prntscr.com/tjhiqx
    11. Select “External” and click “Create” http://prntscr.com/tjhj36
    12. Enter App name and click “Save” http://prntscr.com/tjijw4, http://prntscr.com/tjhlp0
    13. Click “Credentials” menu item http://prntscr.com/tjhlz2
    14. Click “+Create credentials” and select “OAuth client ID” http://prntscr.com/tjhmg4
    15. Select “Web application” application type and enter name. Leave section below empty for now. Click “Create” http://prntscr.com/tjhn1p
    16. Note that for now there is a limit in 100 logins until app will require verification. Below you can see client ID and client secret. You will need them in the next steps. http://prntscr.com/tjhr3k
    17. Next go to your salesforce org’s main setup, type “auth” in search field, select “Auth. Providers” item and click “New” button http://prntscr.com/tjhveq
    18. Select “Google” provider type http://prntscr.com/tjhvrs
    19. Enter provider name, consumer key (google client ID mentioned earlier) and consumer secret (google client secret). In Authorize Endpoint URL field enter following: https://accounts.google.com/o/oauth2/auth?access_type=offline&approval_prompt=force , in Token Endpoint URL enter https://accounts.google.com/o/oauth2/accessToken , in Default Scopes enter openid email profile https://www.googleapis.com/auth/drive , then click “Save” http://prntscr.com/tjhy19
    20. Enter salesforce org’s domen URL in Authorized JavaScript origins section of a google credentials page, enter URL’s from Salesforce Configuration section in Authorized redirect URLs section of a google credentials page http://prntscr.com/tjhyfa, http://prntscr.com/tjhzef
    21. Go again to your salesforce org’s main setup, type “named” in search field, select “Named Credentials” item and click “New Named Credential” button http://prntscr.com/tji0sk
    22. Enter label and name, in URL field enter https://www.googleapis.com , select Identity Type “Per User”, Authorization Protocol “OAuth 2.0”, in Authentication Provider field select previously created provider, in Scope field enter openid email profile https://www.googleapis.com/auth/drive , and make sure all checkboxes selected as shown on screenshot http://prntscr.com/tji26u
    23. Because of Start Authentication Flow on Save checkbox from previous step you will be redirected to google’s select account page and after to google’s authentication page, where you need to click “Advanced” link and then click on “Go to salesforce.com” link and confirm all the following steps http://prntscr.com/tji388, http://prntscr.com/tji3cp
    24. After confirming you will be redirected back to SF page and Administration Authentication Status will be changed to “Authenticated as...” http://prntscr.com/tji421
    25. Go to SF main setup, type “custom” in search field, select “Custom Metadata Types”, find “CB Google Drive Connect Settings” and click “Manage Records” link http://prntscr.com/tji5yx
    26. Find “CBGDConnect” item (there is should be only one) and click “Edit” link http://prntscr.com/tji663
    27. In Named Credential Name field enter name of previously created Named Credential, then click “Save” http://prntscr.com/tji6gt
    28. Add “CB Connect” permission set to needed users http://prntscr.com/tji768
    29. In order to login each user need to go to their settings and create new Authentication Settings for External Systems http://prntscr.com/tji4e4, http://prntscr.com/tji4ne
    30. Set up as shown on screenshot, make sure that “Start Authentication Flow on Save” checkbox is checked, then click “Save”, repeat google’s authentication procedure (each user can login to a different google drive) http://prntscr.com/tji546
    31. Check if Google Drive connection works: http://prntscr.com/tjj9k7

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