# Google App Engine

## Installation

- Extract the [downloaded ZIP file](https://cloud.google.com/appengine/downloads) to ~/dev.
- In `~/.bash_custom`, add `~/dev/google_appengine` to the PATH.

## Hello World

Create the following directory structure:

```
helloworld
|_ app.yaml
|_ helloworld.py
```

app.yaml:
```yaml
version: 1
runtime: python27
api_version: 1
threadsafe: true

handlers:
- url: /.*
  script: helloworld.app
```

helloworld.py:
```python
import webapp2

class MainPage(webapp2.RequestHandler):
    def get(self):
        self.response.headers['Content-Type'] = 'text/plain'
        self.response.write('Groobus, Smelt!')

app = webapp2.WSGIApplication([
    ('/', MainPage),
], debug=True)
```

To run the app with the dev server:

```
dev_appserver.py helloworld/
```
