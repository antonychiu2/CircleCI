# Introduction
This is an example that demonstrate the ease of use of ASoC's powerful REST API capabilities. 

Within 7 simple REST API method calls, I was able to get a SAST scan submitted into ASoC for static analysis and get scan result/report back. 


# ASoC REST API used:

`Account/ApiKeyLogin`

`/FileUpload`

`/Scans/StaticAnalyzer`

`/Scans/$scan_ID/Executions`

`/Reports/Security/Scan/$scan_ID`

`/Reports/$report_ID`

`/Reports/Download/$report_ID`

# ASoC's full REST API list:
https://cloud.appscan.com/swagger/ui/index

# To set this up, you also need to first define Environment variables for the Circle CI project:

![1](https://user-images.githubusercontent.com/5158535/118554892-47b75b00-b71f-11eb-8892-9b2b90e65dbf.png)


# Screenshot of the pipeline steps:
![2](https://user-images.githubusercontent.com/5158535/118554911-4dad3c00-b71f-11eb-99d4-72aff2414c50.png)



# The report is automatically saved as a Circle CI artifact:
![3](https://user-images.githubusercontent.com/5158535/118554932-53a31d00-b71f-11eb-93f7-1d226895ea1f.png)


# Let's check on the "html" report:
![4](https://user-images.githubusercontent.com/5158535/118554941-56057700-b71f-11eb-8457-41555f608789.png)

