To make an http text response application you must do this:

```python 
from yungestWeb import *

app = App()

def http_response(request: Request):
    return HttpResponse(request, "{string or var}")

routes = [
    Path("/{any or empty}", http_response)
]

app.set_routes(routes)
run_webapp("127.0.0.1", 8080, app)
```