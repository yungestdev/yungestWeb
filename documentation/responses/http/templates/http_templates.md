To make an http template response application you must do this:

```python 
from yungestWeb import *

app = App()

def http_response(request: Request):
    return HttpResponse(request, render_html("html_filename"))

routes = [
    Path("/{any or empty}", http_response)
]

app.set_routes(routes)
app.run("127.0.0.1", 8080, app)
```