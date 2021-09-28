# REPOSITORIO MME 2021/2022

Write-host 
           "======================="
Write-host "(                     )"
Write-host "(                     )"
Write-host "(       MENU          )"
Write-host "(                     )"
Write-host "(                     )"
Write-host "======================="

Write-host "1.convierte de binario a decimal"
Write-host "2.convierte de hexadecimala binario"
Write-host "3.convierte de hexadecimala a octal"
WriTe-host "4. convierte de octal a binaro"


$var=Read-Host "seleciona opcion"
if($var-eq 1)
{
$binario=Read-Host "dime el numero binario"
$valor=[convert]::toint32($binario,2)
"el numero es..."+$valor
}
if($var-eq 2)
{
$hexa=Read-Host "dime el numero hexadecimal"
$valor=[convert]::ToInt32($hexa,16)
$valor=[convert]::ToString($valor,2)
"el valor es"+$valor
}
if($var-eq 3)
{
$rz=Read-Host "dime el numero e hexadecimal"
$amd=[convert]::ToInt32($rz,16)
$amd=[convert]::ToString($amd,8)
"el valor es..."+$amd
}
if($var-eq 4)
{
$mrc=Read-Host "dime el número en octal"
$octa=[convert]::Toint32($mrc,8)
$octa=[convert]::ToString($octa,2)
"el valor es..."+$octa
}
