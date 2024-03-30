# Example SPA using OIDC+PKCE

This example demonstrates how to use OIDC+PKCE in a SPA.  The same logic is
also usable for backend and mobile applications.

Using PKCE alleviates us from having to know/store secrets when implementing
login flows.

Note that session management will still need to be implemented and is outside
the scope of this example.

# Running this

1. Modify the provider list with data pertaining to your identity provider
    - This involves registering an `application` to use OIDC+PKCE.
      You'll need to specify the URL of the `application` and then get back a
      `Client ID`.

2. Run a webserver to serve the page up and visit it
    - ```shell
      python3 -m http.server
      # visit http://localhost:8000
      ```

# License

```
MIT License

Copyright (c) 2024 coauthnz

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
