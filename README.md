<div align="center">

## \*\*\*Form Flash\*\*\*


</div>

### Description

This code makes your form window flash like Aol's Instant Messanger when it receives a message.
 
### More Info
 
make a timer and set the interval to 3000.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Ben Doherty](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ben-doherty.md)
**Level**          |Unknown
**User Rating**    |3.6 (50 globes from 14 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Windows API Call/ Explanation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows-api-call-explanation__1-39.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ben-doherty-form-flash__1-2090/archive/master.zip)

### API Declarations

```
private declare function FlashWindow lib "user32" alias "FlashWindow" (ByVal hWnd as long, ByVal bInvert as long) as long
```


### Source Code

```
Private sub timer1_timer()
dim nReturnValue as integer
nReturnValue = FlashWindow(form1.hWnd, true)
end sub
```

