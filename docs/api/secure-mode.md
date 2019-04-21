# `secure mode`

Changes the default values of following `webPreferences`:
- `sandbox: true`
- `contextIsolation: true`
- `nativeWindowOpen: true`
- `enableRemoteModule: false`

Removes the ability to use the following `webPreferences`:
- `nodeIntegration`
- `nodeIntegrationInWorker`

When the following events are unhandled, `event.preventDefault()` is called implicitly:
- `new-window`
- `will-attach-webview`

When no handler is set using `session.setPermissionRequestHandler()`, it behaves as if `callback(false)` was called.
