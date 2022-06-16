To make a json response application you must do this:

```python 
from yungestWeb import *

app = App()

def json_response(request: Request):
    return JsonResponse(request, {json_content})

routes = [
    Path("/{any or empty}", json_response)
]

app.set_routes(routes)
app.run("127.0.0.1", 8080, app)
```