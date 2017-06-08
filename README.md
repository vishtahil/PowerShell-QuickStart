# PowerShell-QuickStart


# Template strings
```
$FirstName = "Ken"
$LastName = "Myer"
$Title = "Accountant"
$Department = "Financial Services"

Write-Host "$FirstName $LastName is an $Title in $Department."

$var2=($var1=1)+1
```
# Insert characters to the file
```
${C:\some_file.txt} = "vishal"
```

# If condition
```
[int] $var1=10
[int] $var2 =20

IF($var1 -le $var2){
  $var1
  }

```

# Powershell conditional
```
Get-ChildItem | Where-Object {($_.Name -like "*angula*")}| ForEach-Object {$_.Name}
```

# For Each Object
```
Get-ChildItem | ForEach-Object {write-host $_.Name}

#For Loop
For ([int]$i=0; $i -le 10; $i++) {
   Write-Host "10 * $i = " + (10 * $i)

    }
```
# Arrays
```
$colors = @("Red","Orange","Yellow","Green","Blue","Indigo","Violet")
For ($i=0; $i -lt $colors.Length; $i++) {
   Write-Host $colors[$i]
    }
```
# DO While
```
$i=1
Do {
    $i
    $i++
    }
While ($i -le 10)
```
# File Handling
```
Get-ChildItem | Out-File -FilePath "C:\dev\gsp\vishal.txt"
Get-Content C:\dev\gsp\vishal.txt
Clear-Host
cat C:\dev\gsp\vishal.txt
notepad
set-location -path "folderlocation"
```
# Functions
```
function Add-Numbers
{
 $args[0] + $args[1]
}

Add-Numbers 1 10
```
