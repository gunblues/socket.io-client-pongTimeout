# socket.io-client-pongTimeout
At bad network, you might want to show "the connection is unstable"
If pong response is slower than pongTimeout value, trigger pong_abnormal event; If pong response is back to normal, trigger pong_normal event


## How to use

```html
<script src="socket.io-pongTimeout-1.3.5.js"></script>
<script>
  //if you don't pass PongTimeout, the default value is 6000
  var socket = io('http://localhost', {pongTimeout: 5000});
  socket.on('pong_abnormal', function(){});
  socket.on('pong_normal', function(){});
</script>
```
