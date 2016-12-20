# PowerShell-QuickStart
Powershell Quick start

#template strings
$FirstName = "Ken"
$LastName = "Myer"
$Title = "Accountant"
$Department = "Financial Services"

Write-Host "$FirstName $LastName is an $Title in $Department."

$var2=($var1=1)+1

#appending characters to the file
${C:\some_file.txt} = "vishal"

[int] $var1=10
[int] $var2 =20

$var1
$var2
#if condition
IF($var1 -le $var2){
  $var1
  }
Get-ChildItem

#powershell conditional
Get-ChildItem | Where-Object {($_.Name -like "*angula*")}| ForEach-Object {$_.Name}

#foreach object
Get-ChildItem | ForEach-Object {write-host $_.Name}

#for--loop
For ([int]$i=0; $i -le 10; $i++) {
   Write-Host "10 * $i = " + (10 * $i)

    }

#array
$colors = @("Red","Orange","Yellow","Green","Blue","Indigo","Violet")
For ($i=0; $i -lt $colors.Length; $i++) {
   Write-Host $colors[$i]
    }

#do while
$i=1
Do {
    $i
    $i++
    }
While ($i -le 10)

#file handling
Get-ChildItem | Out-File -FilePath "C:\dev\gsp\vishal.txt"
Get-Content C:\dev\gsp\vishal.txt
Clear-Host
cat C:\dev\gsp\vishal.txt
notepad
set-location -path "folderlocation"

#functions
function Add-Numbers
{
 $args[0] + $args[1]
}

Add-Numbers 1 10

