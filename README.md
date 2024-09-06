# wasm-pack fails to load with raw browser import

Reproduction:

```
wasm-pack build
```

Then launch a server:

```
python3 -m http.server 8888
```

navigate to [http://localhost:8888/](http://localhost:8888/)

open the console and see

```
Failed to load module script: Expected a JavaScript module script but the server responded with a MIME type of "application/wasm". Strict MIME type checking is enforced for module scripts per HTML spec.
```
