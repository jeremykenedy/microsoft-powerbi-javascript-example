# Microsoft PowerBI  Javascript Embedded Example [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Table of Contents:
- [About](#about)
- [API Call Requirements](#api-call-requirements)
- [Examples](#examples)
- [Libraries Used](#Libraries-used)
- [File Tree](#file-tree)
- [Resources](#resources)
- [Notes](#notes)
- [License](#license)

## About
Microsoft Power BI is a suite of business analytics tools that deliver insights throughout your organization.

This is an example of the [powerbi-client API](https://microsoft.github.io/PowerBI-JavaScript/) javascript embeded interface. 

## API Call Requirements
In order to make an API request to Microsoft PowerBI You will need the following basic information for your request (obtained from PowerBI as outline [here](https://github.com/Microsoft/PowerBI-Developer-Samples#step-1---app-registration)):
| Name | Desc | Required|
| :------------ | :------------ | :------------ |
|Embed Token|The API Token that is ties the PowerBI Account to the request.| YES |
|Embed URL|The URL we will be sending the request to, query params may change based on report type.| YES |
|Dashboard ID|The ID of the dashbord we want.| Dependant on report type |
|Report ID|The ID of the specific report we want.| Dependant on report type |
|Group ID|The ID of the specific report group we want.| Dependant on report type |
|Tile ID|The ID of the dashboard tile report we want.| Dependant on report type |

* Note: There may be more depending on what type of report you want.

## Examples
|Type|Desc|File|Required API Fields|
|:------------|:------------|:------------|:------------|
|Hard Coded|API Call values are hard coded.|[hard-coded-example.html](hard-coded-example.html)|Token, URL, Dashboard ID|
|Form Input Dashboard|API Call values are poplulated from form inputs for a dashboard.|[input-form-dashboard-example.html](input-form-dashboard-example.html)|Token, URL, Dashboard ID|
|Form Input Report|API Call values are poplulated from form inputs for a specific report.|[input-form-report-example.html](input-form-report-example.html)|Token, URL, Report ID, Group ID|

## Libraries Used
* [powerbi.js](https://github.com/Microsoft/PowerBI-JavaScript/blob/master/dist/powerbi.js)
* [powerbi.js](https://github.com/Microsoft/PowerBI-JavaScript/blob/master/dist/powerbi.js)
* [jQuery](https://code.jquery.com/jquery-3.3.1.min.js)

### File Tree
```
microsoft-powerbi-javascript-example
├── .gitignore
├── README.md
├── hard-coded-example.html
├── input-form-dashboard-example.html
├── input-form-report-example.html
├── power-bi.js
└── power-bi.min.js
```

* Tree command can be installed using brew: `brew install tree`
* File tree generated using command `tree -a -I '.git|node_modules|vendor|storage|tests'`

## Resources
* [https://github.com/Microsoft/PowerBI-Developer-Samples](https://github.com/Microsoft/PowerBI-Developer-Samples)
* [https://microsoft.github.io/PowerBI-JavaScript/](https://microsoft.github.io/PowerBI-JavaScript/)
* [https://microsoft.github.io/PowerBI-JavaScript/demo/v2-demo/index.html#](https://microsoft.github.io/PowerBI-JavaScript/demo/v2-demo/index.html#)
* [https://docs.microsoft.com/en-us/rest/api/power-bi/](https://docs.microsoft.com/en-us/rest/api/power-bi/)
* [https://docs.microsoft.com/en-us/rest/api/power-bi/reports/getreport](https://docs.microsoft.com/en-us/rest/api/power-bi/reports/getreport)
* [https://docs.microsoft.com/en-us/rest/api/power-bi/reports/getreports](https://docs.microsoft.com/en-us/rest/api/power-bi/reports/getreports)
* [https://docs.microsoft.com/en-us/power-bi/developer/embedding-content](https://docs.microsoft.com/en-us/power-bi/developer/embedding-content)
* [https://www.youtube.com/watch?v=nfkVljh_9O4](https://www.youtube.com/watch?v=nfkVljh_9O4)
* [https://powerbi.microsoft.com/en-us/blog/intro-pbi-js-api/](https://powerbi.microsoft.com/en-us/blog/intro-pbi-js-api/)

### License
This repository and all the code within it is licensed under the [MIT license](https://opensource.org/licenses/MIT). Enjoy!
