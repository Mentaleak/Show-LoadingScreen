

<img align="left" width="64" height="64" src="https://raw.githubusercontent.com/Mentaleak/Show-LoadingScreen/master/images/loading.ico?token=AFLELQ7CFGVJZV4ULEN3CQS6S46HC"><h1>Show-LoadingScreen</h1>


This is a script that allows a user to show a GUI for loading while their program is working in the background
It can be used both in determinate and indeterminate scenarios
 
 ## Example A
 ![Example A Gif](https://github.com/Mentaleak/Show-LoadingScreen/blob/master/Examples/ExampleA.gif?raw=true)
 ```pwsh
$exampleA = show-LoadingScreen -note "Waiting "
    $i=0
    while($i -lt 99){
    $i++
    Start-Sleep -Milliseconds 50
    }
$exampleA.Close()
```
 ## Example B
 ![Example B Gif](https://github.com/Mentaleak/Show-LoadingScreen/blob/master/Examples/ExampleB.gif?raw=true)
 ```pwsh
$exampleB = show-LoadingScreen
    $i=0
    while($i -lt 99){
    $exampleB.update($i, "$(100-$i)% Left")
    $i++
    Start-Sleep -Milliseconds 50
    }
$exampleB.Close()
```

 ## Example C
 ![Example C Gif](https://github.com/Mentaleak/Show-LoadingScreen/blob/master/Examples/ExampleC.gif?raw=true)
 ```pwsh
$exampleC = show-LoadingScreen
    $i=0
    while($i -lt 99){
    $exampleC.updatePercent($i)
    $i++
    Start-Sleep -Milliseconds 50
    }
$exampleC.Close()
```

 ## Example D
 ![Example D Gif](https://github.com/Mentaleak/Show-LoadingScreen/blob/master/Examples/ExampleD.gif?raw=true)
 ```pwsh
$exampleD = show-LoadingScreen
    $i=0
    while($i -lt 99){
    $exampleD.updateNote("$(100-$i)% Left")
    $i++
    Start-Sleep -Milliseconds 50
    }
$exampleD.Close()
```
