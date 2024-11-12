# PowerShell
## Download file from the internet and save locally
> `md -Force C:\temp; (New-Object System.Net.WebClient).DownloadFile("http://sampleurl.com/samplefile.xml","C:\temp\sample.xml")`

## GREP Like for Powershell
> `Get-ChildItem -Recurse | Select-String -Pattern "search-value"`

## Run Powershell N-number of times
> `for ($i = 1; $i -le 5; $i++) { npx karma start --browsers=ChromeHeadless --single-run=true | Out-File -FilePath ("tests/output_" + (Get-Date -Format "yyyyMMdd_HHmmss") + ".txt") -Append }`
