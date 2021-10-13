# Small websocket server implementation
You can use this program for various uses.
For example, communicate with browser's JavaScript, send command request to minecraft ("/connect HOST:PORT" command).

### example
- [remote_minecraft](https://github.com/atoy322/remote_minecraft)
- developing...

---
## How to install
```shell
pip install thin-ws-server
```
---
## Usage
```python
from thin_ws_server import WebSocketServer

ws = WebSocketServer(8000)  # initialize with port number
ws.accept()  # accept client connection

ws.send(data)  # data: str or bytes
ws.recv()  # returns bytes
```
