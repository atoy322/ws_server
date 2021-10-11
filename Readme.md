# Small websocket server implementation
You can use this program for various way.
For example, communicate with browser's JavaScript, send command request to minecraft ("/connect HOST:PORT" command).

## Usage
```python
from websocket_server import WebSocketServer

ws = WebSocketServer(8000)  # initialize
ws.accept()  # accept client connection

ws.send(data)  # data: str or bytes
ws.recv()  # returns bytes
```

