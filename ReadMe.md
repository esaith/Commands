# PowerShell
## Download file from the internet and save locally
> `md -Force C:\temp; (New-Object System.Net.WebClient).DownloadFile("http://sampleurl.com/samplefile.xml","C:\temp\sample.xml")`

This will download from http://sampleurl.com/samplefile.xml and will save it to C:\temp\sample.xml. This will create the C:\temp directory if it does not exist. If the sample.xml file already exists, it will override it. Modify the URL and save file location as you need.



## GREP Like for Powershell
> `Get-ChildItem -Recurse | Select-String -Pattern "search-value"`



## Run Powershell N-number of times
> `for ($i = 1; $i -le 50; $i++) { npx karma start --browsers=ChromeHeadless --single-run=true | Out-File -FilePath ("tests/output_" + (Get-Date -Format "yyyyMMdd_HHmmss") + ".txt") -Append; Write-Host "Completed ${i} of 50" }`
