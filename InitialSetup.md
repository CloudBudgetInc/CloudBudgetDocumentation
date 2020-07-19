<html>
<body>

<head>
    <meta charset="UTF-8">
    <title>Initial Setup</title>
</head>

<h1 id='pageTop'>Initial Setup</h1>
<div>
    <p>Yuo may need to perform Initial Setup before your org will go live </p>

    <ul>
        <li><a href="InitialSetup.html#init">Installation</a></li>
        <li><a href="InitialSetup.html#populating">Populating</a></li>
    </ul>


    <table style='border-collapse:collapse;table-layout:fixed;width:1029pt'>
        <tr style='height:15.75pt'>
            <td width=37 style='height:15.75pt;width:28pt'>Step</td>
            <td width=192 style='width:144pt'>Title</td>
            <td width=602 style='width:452pt'>Actions</td>
            <td width=169 style='width:127pt'>Screenshots</td>
            <td width=370 style='width:278pt'>How To Document</td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>&nbsp;</td>
            <td>GENERAL SETUP</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>1</td>
            <td>CB Instalation</td>
            <td>Make sure that the CloudBudget2 Base package is on your
                instance (Setup -&gt; Installed Packages)
            </td>
            <td><a href="http://prntscr.com/pl28bv" target="_parent"><span
                    style='color:blue'>http://prntscr.com/pl28bv</span></a></td>
            <td></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>2</td>
            <td>Home page setup</td>
            <td>Setup -&gt; Lightning App Builder View
                &quot;Navigation&quot;<br>
                Activation button, asign App &quot;Navigation&quot; to CloudBu<span
                        style='display:none'>dget2<br>
    Next <br>
    Save</span></td>
            <td><a href="http://prntscr.com/pl2a0d" target="_parent"><span
                    style='color:blue'>http://prntscr.com/pl2a0d</span></a></td>
            <td></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>3</td>
            <td>Initialization</td>
            <td>Home -&gt; Other -&gt; Init Wizard<br>
                Do all the steps. If template is not needed - stop at Posting Rules
            </td>
            <td colspan=2 style='mso-ignore:colspan'>http://prntscr.com/pl2b8p<br>
                https://prnt.sc/qr82rl
            </td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>4</td>
            <td>BY and Periods</td>
            <td>Create another BY (if needed)<br>
                Home -&gt; Main Configurator -&gt; Periods Configuration
            </td>
            <td><a href="http://prntscr.com/pm8ek2" target="_parent"><span
                    style='color:blue'>http://prntscr.com/pm8ek2</span></a></td>
            <td></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>5</td>
            <td>Create additional dimensions</td>
            <td>Create analytical metrics of the client (&quot;Project&quot;
                and &quot;Grant&quot; in the current example)<br>
                Main Configurator -<span style='display:none'>&gt; CB Dimension -&gt;
  Create New<br>
    To display the dimension on the Home page enable &quot;Display on
  Home&quot;<br>
    Setup dimension fields/lookups<br>
    Save</span></td>
            <td><a href="http://prntscr.com/qxad1p" target="_parent"><span
                    style='color:blue'>http://prntscr.com/qxad1p</span></a></td>
            <td><a href="https://cloudbudgetinc.github.io/Docs/Dimension"
                   target="_parent"><span
                    style='color:blue'>https://fallentol.github.io/CloudBudget/CB2/Dimension</span></a>
            </td>
        </tr>
        <tr style='height:31.5pt;mso-xlrowspan:2'>
            <td height=42 colspan=5 style='height:31.5pt;mso-ignore:colspan'></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>&nbsp;</td>
            <td>INITIAL DATA POPULATING</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>1</td>
            <td>COA</td>
            <td>Go to Home -&gt; Accounts. Create Account Subtypes</td>
            <td colspan=2 style='mso-ignore:colspan'></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>2</td>
            <td>COA</td>
            <td>Add needed list of accounts or load them using SF Data Import
                Wizard
            </td>
            <td>http://prntscr.com/qxt9xp<br>
                ht<span style='display:none'>tp://prntscr.com/qxtbi3<br>
    http://prntscr.com/qxtc6t</span></td>
            <td><a
                    href="https://cloudbudgetinc.github.io/Docs/COA#import" target="_parent"><span
                    style='color:blue'>https://fallentol.github.io/CloudBudget/CB2/COA#import</span></a></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>3</td>
            <td>Dimensions</td>
            <td>Fill in a list of organization dimensions/analytics</td>
            <td colspan=2 style='mso-ignore:colspan'></td>
        </tr>
        <tr style='height:31.5pt;mso-xlrowspan:2'>
            <td height=42 colspan=5 style='height:31.5pt;mso-ignore:colspan'></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>&nbsp;</td>
            <td>BUDGET APP SETUP</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>1</td>
            <td>Budget App Template</td>
            <td>Go to Main Configurator -&gt; CB Dimensions -&gt; Budget App
                Template dimension <br>
                and setup custom org <span style='display:none'>analytics<span
                        style='mso-spacerun:yes'> </span></span></td>
            <td colspan=2 style='mso-ignore:colspan'>http://prntscr.com/qxak35<br>
                http://prntscr.com/qxayhb
            </td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>2</td>
            <td>Budget App Amounts</td>
            <td>Setup the same analytics to the &quot;Budget App Amount&quot;
                dimension (the same way)
            </td>
            <td colspan=2 style='mso-ignore:colspan'></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>3</td>
            <td>Calculation Rules</td>
            <td colspan=3 style='mso-ignore:colspan'></td>
        </tr>
        <tr style='height:315.0pt;mso-xlrowspan:20'>
            <td colspan=5 style='height:315.0pt;mso-ignore:colspan'></td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'>&nbsp;</td>
            <td>NEW CUSTOM USER</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr style='height:15.75pt'>
            <td style='height:15.75pt'></td>
            <td>Add new User</td>
            <td>Add Permission Set named
                &quot;CloudBudget2PermissionsSet&quot; to simple User
            </td>
            <td><a href="http://prntscr.com/pwass3" target="_parent"><span
                    style='color:blue'>http://prntscr.com/pwass3</span></a></td>
            <td></td>
        </tr>
    </table>

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

    tr {
        mso-height-source: auto;
    }

    col {
        mso-width-source: auto;
    }

    br {
        mso-data-placement: same-cell;
    }

    .style0 {
        mso-number-format: General;
        text-align: general;
        vertical-align: bottom;
        white-space: nowrap;
        mso-rotate: 0;
        mso-background-source: auto;
        mso-pattern: auto;
        color: black;
        font-size: 10.0pt;
        font-weight: 400;
        font-style: normal;
        text-decoration: none;
        font-family: Arial;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        border: none;
        mso-protection: locked visible;
        mso-style-name: Normal;
        mso-style-id: 0;
    }

    td {
        mso-style-parent: style0;
        padding-top: 1px;
        padding-right: 1px;
        padding-left: 1px;
        mso-ignore: padding;
        color: black;
        font-size: 10.0pt;
        font-weight: 400;
        font-style: normal;
        text-decoration: none;
        font-family: Arial;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        mso-number-format: General;
        text-align: general;
        vertical-align: bottom;
        border: none;
        mso-background-source: auto;
        mso-pattern: auto;
        mso-protection: locked visible;
        white-space: nowrap;
        mso-rotate: 0;
    }

    .xl65 {
        mso-style-parent: style0;
        color: #FFE599;
        background: #351C75;
        mso-pattern: #351C75 none;
    }

    .xl66 {
        mso-style-parent: style0;
        color: #FFE599;
        font-size: 14.0pt;
        font-weight: 700;
        background: #351C75;
        mso-pattern: #351C75 none;
    }

    .xl67 {
        mso-style-parent: style0;
        color: black;
    }

    .xl68 {
        mso-style-parent: style0;
        color: black;
        background: yellow;
        mso-pattern: yellow none;
    }

    .xl69 {
        mso-style-parent: style0;
        background: #D9EAD3;
        mso-pattern: #D9EAD3 none;
    }

    .xl70 {
        mso-style-parent: style0;
        background: #CFE2F3;
        mso-pattern: #CFE2F3 none;
    }

    .xl71 {
        mso-style-parent: style0;
        background: #F4CCCC;
        mso-pattern: #F4CCCC none;
    }

    .xl72 {
        mso-style-parent: style0;
        color: #FFF2CC;
        background: #20124D;
        mso-pattern: #20124D none;
    }

    .xl73 {
        mso-style-parent: style0;
        color: yellow;
        background: #0B5394;
        mso-pattern: #0B5394 none;
    }

    .xl74 {
        mso-style-parent: style0;
        color: black;
        font-weight: 700;
        background: #D0E0E3;
        mso-pattern: #D0E0E3 none;
    }

    .xl75 {
        mso-style-parent: style0;
        color: black;
        font-weight: 700;
        background: #CCCCCC;
        mso-pattern: #CCCCCC none;
    }

    .xl76 {
        mso-style-parent: style0;
        color: windowtext;
        font-weight: 700;
        background: #CCCCCC;
        mso-pattern: #CCCCCC none;
    }

    .xl77 {
        mso-style-parent: style0;
        color: black;
        background: #D0E0E3;
        mso-pattern: #D0E0E3 none;
    }

    .xl78 {
        mso-style-parent: style0;
        color: black;
        background: #CCCCCC;
        mso-pattern: #CCCCCC none;
    }

    .xl79 {
        mso-style-parent: style0;
        color: black;
        background: #D9D2E9;
        mso-pattern: #D9D2E9 none;
    }

    .xl80 {
        mso-style-parent: style0;
        color: black;
        background: #CFE2F3;
        mso-pattern: #CFE2F3 none;
    }

    .xl81 {
        mso-style-parent: style0;
        color: black;
        background: #F4CCCC;
        mso-pattern: #F4CCCC none;
    }

    .xl82 {
        mso-style-parent: style0;
        color: blue;
        text-decoration: underline;
        text-underline-style: single;
    }

    .xl83 {
        mso-style-parent: style0;
        color: black;
        white-space: normal;
    }

    .xl84 {
        mso-style-parent: style0;
        color: black;
        background: #D9EAD3;
        mso-pattern: #D9EAD3 none;
    }

    .xl85 {
        mso-style-parent: style0;
        text-align: left;
        background: white;
        mso-pattern: white none;
    }

    .xl86 {
        mso-style-parent: style0;
        color: black;
        text-align: right;
    }

    .xl87 {
        mso-style-parent: style0;
        font-weight: 700;
        background: #D9EAD3;
        mso-pattern: #D9EAD3 none;
    }

    .xl88 {
        mso-style-parent: style0;
        color: black;
        background: #FFF2CC;
        mso-pattern: #FFF2CC none;
    }

    .xl89 {
        mso-style-parent: style0;
        color: windowtext;
    }

    .xl90 {
        mso-style-parent: style0;
        color: #FFE599;
        font-size: 11.0pt;
        font-family: Slack-Lato;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        text-align: left;
        background: #741B47;
        mso-pattern: #741B47 none;
    }

    .xl91 {
        mso-style-parent: style0;
        font-size: 11.0pt;
    }

    .xl92 {
        mso-style-parent: style0;
        font-size: 23.0pt;
        font-family: Roboto;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        background: white;
        mso-pattern: white none;
    }

    .xl93 {
        mso-style-parent: style0;
        font-size: 11.0pt;
        text-decoration: underline;
        text-underline-style: single;
    }

    .xl94 {
        mso-style-parent: style0;
        color: black;
        font-size: 12.0pt;
        font-weight: 700;
    }

    .xl95 {
        mso-style-parent: style0;
        color: black;
        font-weight: 700;
    }

    .xl96 {
        mso-style-parent: style0;
        font-family: Roboto;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        background: white;
        mso-pattern: white none;
    }

    .xl97 {
        mso-style-parent: style0;
        color: black;
        border: none;
    }

    .xl98 {
        mso-style-parent: style0;
        color: #9876AA;
        background: #2B2B2B;
        mso-pattern: #2B2B2B none;
    }

    .xl99 {
        mso-style-parent: style0;
        color: #1D1C1D;
        font-size: 11.0pt;
        font-family: Slack-Lato;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        text-align: left;
        background: white;
        mso-pattern: white none;
    }

    .xl100 {
        mso-style-parent: style0;
        color: #222222;
        font-family: Publico;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        text-align: center;
        background: white;
        mso-pattern: white none;
        white-space: normal;
    }

    .xl101 {
        mso-style-parent: style0;
        color: red;
        font-size: 18.0pt;
        font-weight: 700;
        background: black;
        mso-pattern: black none;
    }

    .xl102 {
        mso-style-parent: style0;
        color: #EFEFEF;
        background: #85200C;
        mso-pattern: #85200C none;
        white-space: normal;
    }

    .xl103 {
        mso-style-parent: style0;
        color: #FFE599;
        font-size: 18.0pt;
        text-align: left;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl104 {
        mso-style-parent: style0;
        color: #EFEFEF;
        background: #85200C;
        mso-pattern: #85200C none;
    }

    .xl105 {
        mso-style-parent: style0;
        color: #FFE599;
        font-size: 18.0pt;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl106 {
        mso-style-parent: style0;
        color: #FFE599;
        font-size: 11.0pt;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl107 {
        mso-style-parent: style0;
        color: black;
        text-align: left;
    }

    .xl108 {
        mso-style-parent: style0;
        color: #FFE599;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl109 {
        mso-style-parent: style0;
        color: #A61C00;
        background: #FFF2CC;
        mso-pattern: #FFF2CC none;
    }

    .xl110 {
        mso-style-parent: style0;
        color: #1D1C1D;
        font-size: 11.0pt;
        font-family: Slack-Lato;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        text-align: left;
        background: #F8F8F8;
        mso-pattern: #F8F8F8 none;
        white-space: normal;
    }

    .xl111 {
        mso-style-parent: style0;
        color: #16325C;
        font-weight: 700;
        background: white;
        mso-pattern: white none;
    }

    .xl112 {
        mso-style-parent: style0;
        color: #222222;
        font-weight: 700;
        background: white;
        mso-pattern: white none;
    }

    .xl113 {
        mso-style-parent: style0;
        color: black;
        font-weight: 700;
        white-space: normal;
    }

    .xl114 {
        mso-style-parent: style0;
        color: #D0E0E3;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl115 {
        mso-style-parent: style0;
        color: black;
        font-size: 14.0pt;
        font-weight: 700;
    }

    .xl116 {
        mso-style-parent: style0;
        color: black;
        font-size: 14.0pt;
        white-space: normal;
    }

    .xl117 {
        mso-style-parent: style0;
        text-align: left;
        background: #FFF2CC;
        mso-pattern: #FFF2CC none;
    }

    .xl118 {
        mso-style-parent: style0;
        color: black;
        font-size: 14.0pt;
        font-weight: 700;
        white-space: normal;
    }

    .xl119 {
        mso-style-parent: style0;
        color: black;
        font-size: 14.0pt;
        background: lime;
        mso-pattern: lime none;
        white-space: normal;
    }

    .xl120 {
        mso-style-parent: style0;
        color: #080707;
        text-align: left;
        background: #F3F2F2;
        mso-pattern: #F3F2F2 none;
    }

    .xl121 {
        mso-style-parent: style0;
        color: black;
        font-size: 14.0pt;
        background: yellow;
        mso-pattern: yellow none;
        white-space: normal;
    }

    .xl122 {
        mso-style-parent: style0;
        color: #080707;
        text-align: left;
        background: #F3F2F2;
        mso-pattern: #F3F2F2 none;
        white-space: normal;
    }

    .xl123 {
        mso-style-parent: style0;
        color: black;
        mso-number-format: "dd\/mm\/yyyy";
    }

    .xl124 {
        mso-style-parent: style0;
        color: black;
        font-size: 14.0pt;
        background: red;
        mso-pattern: red none;
        white-space: normal;
    }

    .xl125 {
        mso-style-parent: style0;
        color: #CC7832;
        background: #2B2B2B;
        mso-pattern: #2B2B2B none;
    }

    .xl126 {
        mso-style-parent: style0;
        color: windowtext;
        white-space: normal;
    }

    .xl127 {
        mso-style-parent: style0;
        color: #E8BF6A;
        font-weight: 700;
        font-style: italic;
        background: #2B2B2B;
        mso-pattern: #2B2B2B none;
    }

    .xl128 {
        mso-style-parent: style0;
        color: #993300;
        font-size: 11.0pt;
        font-family: DSCDefaultFontRegular;
        mso-generic-font-family: auto;
        mso-font-charset: 0;
        background: white;
        mso-pattern: white none;
    }

    .xl129 {
        mso-style-parent: style0;
        color: #FFF2CC;
        background: #134F5C;
        mso-pattern: #134F5C none;
        white-space: normal;
    }

    .xl130 {
        mso-style-parent: style0;
        color: #FFF2CC;
        background: #134F5C;
        mso-pattern: #134F5C none;
    }

    .xl131 {
        mso-style-parent: style0;
        color: black;
        background: #EA9999;
        mso-pattern: #EA9999 none;
        white-space: normal;
    }

    .xl132 {
        mso-style-parent: style0;
        color: black;
        background: #EA9999;
        mso-pattern: #EA9999 none;
    }

    .xl133 {
        mso-style-parent: style0;
        color: black;
        text-align: left;
        white-space: normal;
    }

    .xl134 {
        mso-style-parent: style0;
        color: black;
        background: #C9DAF8;
        mso-pattern: #C9DAF8 none;
        white-space: normal;
    }

    .xl135 {
        mso-style-parent: style0;
        color: black;
        background: #C9DAF8;
        mso-pattern: #C9DAF8 none;
    }

    .xl136 {
        mso-style-parent: style0;
        color: black;
        background: #FFF2CC;
        mso-pattern: #FFF2CC none;
        white-space: normal;
    }

    .xl137 {
        mso-style-parent: style0;
        color: black;
        font-weight: 700;
        background: #FFF2CC;
        mso-pattern: #FFF2CC none;
    }

    .xl138 {
        mso-style-parent: style0;
        color: black;
        mso-number-format: "d\\-m";
        white-space: normal;
    }

    .xl139 {
        mso-style-parent: style0;
        text-align: left;
        background: white;
        mso-pattern: white none;
        white-space: normal;
    }

    .xl140 {
        mso-style-parent: style0;
        color: black;
        mso-number-format: "d\\-m";
    }

    .xl141 {
        mso-style-parent: style0;
        color: black;
        text-align: right;
        white-space: normal;
    }

    .xl142 {
        mso-style-parent: style0;
        color: #080707;
        text-align: left;
        background: white;
        mso-pattern: white none;
    }

    .xl143 {
        mso-style-parent: style0;
        color: red;
    }

    .xl144 {
        mso-style-parent: style0;
        color: red;
        white-space: normal;
    }

    .xl145 {
        mso-style-parent: style0;
        color: #CC0000;
    }

    .xl146 {
        mso-style-parent: style0;
        color: #CC0000;
        white-space: normal;
    }

    .xl147 {
        mso-style-parent: style0;
        color: #D9EAD3;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl148 {
        mso-style-parent: style0;
        color: black;
        mso-number-format: "Short Time";
    }

    .xl149 {
        mso-style-parent: style0;
        color: black;
        text-align: center;
    }

    .xl150 {
        mso-style-parent: style0;
        color: #FFF2CC;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl151 {
        mso-style-parent: style0;
        color: #434343;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl152 {
        mso-style-parent: style0;
        color: black;
        background: #434343;
        mso-pattern: #434343 none;
    }

    .xl153 {
        mso-style-parent: style0;
        color: black;
        vertical-align: top;
    }

</style>


</body>
</html>