# socket.io-client-pongTimeout
if pong is slower than pongTimeout value, trigger pong_abnormal event; if pong is back to normal, trigger pong_normal event


## How to use

```html
<script src="socket.io-pongTimeout-1.3.5.js"></script>
<script>
  var socket = io('http://localhost', {pongTimeout: 5000});
  socket.on('pong_abnormal', function(){});
  socket.on('pong_normal', function(data){});
</script>
```
