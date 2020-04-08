# Show-LoadingScreen
 
 ```pwsh
$exampleA = show-LoadingScreen -note "Waiting "
    $i=0
    while($i -lt 99){
    $i++
    Start-Sleep -Milliseconds 50
    }
$exampleA.Close()
```

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
