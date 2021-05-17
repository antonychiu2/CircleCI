This is an example that demonstrate the ease of use of ASoC's powerful REST API capabilities. Within 7 simple REST API method calls, I was able to get a SAST scan submitted into ASoC for static analysis and get scan result/report back. 

Here is the link to the Circle CI config.yml file:
https://github.com/antonychiu2/CircleCI

ASoC REST API used:

Account/ApiKeyLogin
/FileUpload
/Scans/StaticAnalyzer
/Scans/$scan_ID/Executions
/Reports/Security/Scan/$scan_ID
/Reports/$report_ID
/Reports/Download/$report_ID

ASoC's full REST API list:
https://cloud.appscan.com/swagger/ui/index

To set this up, you also need to first define Environment variables for the Circle CI project:


Screenshot of the pipeline steps:



The report is automatically saved as a Circle CI artifact:


If I click on the "html" report:

