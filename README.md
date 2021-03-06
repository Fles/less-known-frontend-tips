# Less known frontend tips

## Hiding an HTML element 
By using the attribute hidden , you can easily hide an HTML element natively. As a result, that element won’t be displayed on the web page.

```<p hidden>This paragraph won't show up. It's hidden by HTML.</p>```

## Use the inset shorthand in CSS
If top , left , right , and bottom properties have the same value, you can just use the property inset instead and your code will look much cleaner.

```
.dontDoThis{
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

.doLikeThis{
  position: absolute;
  inset: 0;
}
```

## Detect internet speed
```navigator.connection.downlink;```

## Vibrate your phone

```window.navigator.vibrate(500);```

## Disable pull to refresh
```
body{
 overscroll-behavior-y: contain;
}
```

## Prevent the user from pasting text
```
<input type="text"></input><script>//selecting the input.
  const input = document.querySelector('input');
  
//prevent the user to paste text by using the paste eventListener.
  input.addEventListener("paste", function(e){
    e.preventDefault()
  })
  
</script>
```
