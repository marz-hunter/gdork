# Google Dorks for Bug Bounty

A list of Google Dorks for Bug Bounty, Web Application Security, and Pentesting

[Live Tool](https://taksec.github.io/google-dorks-bug-bounty/)

[![tool screenshot](https://github.com/TakSec/google-dorks-bug-bounty/assets/27094033/3ff009d7-f402-4eb2-8321-ce22eeeb5605)](https://taksec.github.io/google-dorks-bug-bounty/)

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/TakSec.svg?style=social&label=Follow%20%40TakSec)](https://twitter.com/TakSec)
</p>

---

### Broad domain search w/ negative search <!--omit-->

```
site:example.com -www -shop -share -ir -mfa
```

### PHP extension w/ parameters

```
site:example.com ext:php inurl:?
```

### API Endpoints

```
site:example[.]com inurl:api | site:*/rest | site:*/v1 | site:*/v2 | site:*/v3
```

### Juicy Extensions

```
site:"example[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess | ext:json
```

### High % inurl keywords

```
inurl:conf | inurl:env | inurl:cgi | inurl:bin | inurl:etc | inurl:root | inurl:sql | inurl:backup | inurl:admin | inurl:php site:example[.]com
```

### Server Errors

```
inurl:"error" | intitle:"exception" | intitle:"failure" | intitle:"server at" | inurl:exception | "database error" | "SQL syntax" | "undefined index" | "unhandled exception" | "stack trace" site:example[.]com
```

### XSS prone parameters

```
inurl:q= | inurl:s= | inurl:search= | inurl:query= | inurl:keyword= | inurl:lang= inurl:& site:example.com
```

### Open Redirect prone parameters

```
inurl:url= | inurl:return= | inurl:next= | inurl:redirect= | inurl:redir= | inurl:ret= | inurl:r2= | inurl:page= inurl:& inurl:http site:example.com
```

### SQLi Prone Parameters

```
inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:example.com
```

### SSRF Prone Parameters

```
inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:example.com
```

### LFI Prone Parameters

```
inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:example.com
```

### RCE Prone Parameters

```
inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:example.com
```

### File upload endpoints

```
site:example.com ”choose file”
```

### API Docs

```
inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"example[.]com"
```

### Login Pages

```
inurl:login | inurl:signin | intitle:login | intitle:signin | inurl:secure site:example[.]com
```

### Test Environments

```
inurl:test | inurl:env | inurl:dev | inurl:staging | inurl:sandbox | inurl:debug | inurl:temp | inurl:internal | inurl:demo site:example.com
```

### Sensitive Documents

```
site:example.com ext:txt | ext:pdf | ext:xml | ext:xls | ext:xlsx | ext:ppt | ext:pptx | ext:doc | ext:docx
intext:“confidential” | intext:“Not for Public Release” | intext:”internal use only” | intext:“do not distribute”
```

### Sensitive Parameters

```
inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:example[.]com
```

### Adobe Experience Manager (AEM)

```
inurl:/content/usergenerated | inurl:/content/dam | inurl:/jcr:content | inurl:/libs/granite | inurl:/etc/clientlibs | inurl:/content/geometrixx | inurl:/bin/wcm | inurl:/crx/de site:example[.]com
```

### Disclosed XSS and Open Redirects

```
site:openbugbounty.org inurl:reports intext:"example.com"
```

### Google Groups

```
site:groups.google.com "example.com"
```

### Code Leaks

```
site:pastebin.com "example.com"
```

```
site:jsfiddle.net "example.com"
```

```
site:codebeautify.org "example.com"
```

```
site:codepen.io "example.com"
```

### Cloud Storage

```
site:s3.amazonaws.com "example.com"
```

```
site:blob.core.windows.net "example.com"
```

```
site:googleapis.com "example.com"
```

```
site:drive.google.com "example.com"
```

```
site:dev.azure.com "example[.]com"
```

```
site:onedrive.live.com "example[.]com"
```

```
site:digitaloceanspaces.com "example[.]com"
```

```
site:sharepoint.com "example[.]com"
```

```
site:s3-external-1.amazonaws.com "example[.]com"
```

```
site:s3.dualstack.us-east-1.amazonaws.com "example[.]com"
```

```
site:dropbox.com/s "example[.]com"
```

```
site:box.com/s "example[.]com"
```

```
site:docs.google.com inurl:"/d/" "example[.]com"
```

### JFrog Artifactory

```
site:jfrog.io "example[.]com"
```

### Firebase

```
site:firebaseio.com "example[.]com"
```

### Bug Bounty programs and Vulnerability Disclosure Programs <!--omit-->

```
site:example.com "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"
```

```
site:example.com "bounty"
```

```
site:example.com inurl /bug bounty
```

```
inurl : / security site:example.com
```

```
inurl:security.txt site:example.com
```

```
site:example.com inurl:security "reward"
```

```
site:example.com inurl : /responsible disclosure
```

```
site:example.com inurl : /responsible-disclosure/ reward
```

```
site:example.com inurl : / responsible-disclosure/ swag
```

```
site:example.com inurl : / responsible-disclosure/ bounty
```

```
site:example.com inurl:'/responsible disclosure' hoodie
```

```
site:example.com responsible disclosure swag r=h:com
```

```
site:example.com responsible disclosure hall of fame
```

```
site:example.com inurl:responsible disclosure $50
```

```
responsible disclosure europe site:example.com
```

```
responsible disclosure white hat site:example.com
```

```
white hat program site:example.com
```

```
insite:"responsible disclosure" -inurl:nl site:example.com
```

```
site:example.com intext responsible disclosure
```

```
site:example.com responsible disclosure
```

```
site:example.com responsible disclosure:sites
```

```
site:example.com responsible disclosure r=h:nl
```

```
site:example.com responsible disclosure r=h:uk
```

```
site:example.com responsible disclosure r=h:eu
```

```
site:example.com responsible disclosure bounty r=h:nl
```

```
site:example.com responsible disclosure bounty r=h:uk
```

```
responsible disclosure bounty r=h:eu site:example.com
```

```
responsible disclosure swag r=h:nl site:example.com
```

```
responsible disclosure swag r=h:uk site:example.com
```

```
responsible disclosure swag r=h:eu site:example.com
```

```
responsible disclosure reward r=h:nl site:example.com
```

```
responsible disclosure reward r=h:uk site:example.com
```

```
responsible disclosure reward r=h:eu site:example.com
```

```
site:example.com "powered by bugcrowd" -site:bugcrowd.com
```

```
site:example.com "submit vulnerability report"
```

```
site:example.com "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"
```

```
"responsible disclosure" site:example.com
```

```
intext:"we take security very seriously" site:example.com
```

```
inurl:'vulnerability-disclosure-policy' reward site:example.com
```

```
site:example.com intext:Vulnerability Disclosure
```

```
site:example.com intext:security report reward
```

```
site:example.com intext:responsible disclosure reward
```

```
site:example.com "security vulnerability" "report"
```

```
site:example.com inurl"security report"
```

```
site:example.com "responsible disclosure" university
```

```
site:example.com inurl:/responsible-disclosure/ university
```

```
site:example.com buy bitcoins "bug bounty"
```

```
inurl:/security ext:txt "contact" site:example.com
```

```
site:example.com "powered by synack"
```

```
site:example.com intext:responsible disclosure bounty
```

```
site:example.com inurl: private bugbountyprogram
```

```
site:example.com inurl:/.well-known/security ext:txt
```

```
site:example.com inurl:/.well-known/security ext:txt intext:hackerone
```

```
site:example.com inurl:/.well-known/security ext:txt -hackerone -bugcrowd -synack -openbugbounty
```

```
site:example.com inurl:reporting-security-issues
```

```
site:example.com inurl:security-policy.txt ext:txt
```

```
inurl:bug inurl:bounty site:example.com
```

```
inurl:bounty site:example.com
```

```
intext:security report reward site:example.com
```

```
intext:security report monetary inurl:security site:example.com
```

```
intext:security report reward inurl:report site:example.com
```

```
inurl: bounty site:example.com
```

```
site:example.com inurl:bug inurl:bounty
```

```
intext:security report reward site:example.com
```

```
site:example.com "vulnerability reporting policy"
```

```
site:example.com "van de melding met een minimum van een" -site:responsibledisclosure.nl
```
 
```
site:example.com inurl:responsible-disclosure-policy
```

```
site:example.com "If you believe you've found a security vulnerability"
```

```
site:example.com intext:"BugBounty" and intext:"BTC" and intext:"reward"
```

```
site:example.com intext:bounty inurl:/security
```

```
site:example.com inurl:"bug bounty" and intext:"€" and inurl:/security
```

```
site:example.com inurl:"bug bounty" and intext:"$" and inurl:/security
```

```
site:example.com inurl:"bug bounty" and intext:"USD" and inurl:/security
```

```
site:example.com inurl:/security.txt "mailto*" -github.com  -wikipedia.org -portswigger.net -magento
```

```
site:example.com /trust/report-a-vulnerability
```

```
site:example.com intext:security report vulnerability
```

```
"cms" bug bounty site:example.com
```

```
site:example.com "If you find a security issue"  "reward"
```

```
site:example.com "responsible disclosure" intext:"you may be eligible for monetary compensation"
```

```
site:example.com inurl: "responsible disclosure", "bug bounty", "bugbounty"
```

```
site:example.com intext: we offer a bounty
```

```
responsible disclosure inurl:in
```

```
site:*/security.txt "bounty"
```

```
site:example.com inurl:bug bounty intext:"EUR"
```

```
site:example.com inurl:bug bounty intext:"$"
```

```
site:example.com inurl:responsible disclosure intext:"USD"
```


### Apache Server Status Exposed <!--omit-->

```
site:example.com /server-status apache
```

### WordPress <!--omit-->

```
inurl:/wp-admin/admin-ajax.php site:example.com
```

### Drupal <!--omit-->

```
intext:"Powered by" & intext:Drupal & inurl:user site:example.com
```

### Joomla <!--omit-->

```
site:*/joomla/login site:example.com
```


---

Medium articles for more dorks:

https://thegrayarea.tech/5-google-dorks-every-hacker-needs-to-know-fed21022a906

https://infosecwriteups.com/uncover-hidden-gems-in-the-cloud-with-google-dorks-8621e56a329d

https://infosecwriteups.com/10-google-dorks-for-sensitive-data-9454b09edc12

Top Parameters:

https://github.com/lutfumertceylan/top25-parameter

Proviesec dorks:

https://github.com/Proviesec/google-dorks
