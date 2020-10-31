# hibp_async_js_checker

A basic library scoped at the window level to query **Have I Been Pwned** (`https://api.pwnedpasswords.com/range/`) for compromised passwords.

NOTE: This repository is **deprecated** and **archived**.
## API
This sets `window.HIBPChecker` to `hibpLibrary()`. This has a number of functions:

- `function` `sha1(str)`
- `function` `isBlank(str)`
- `function` `httpGet(url)`
- `async` `function` `httpGetAsync(url)`
- `async` `function` `has_been_pwned(password)` - uses `httpGetAsync()` query HIBP with the lower half of the SHA1 of the password. Then, returns if the upper half of that SHA1 hash of the password shows up in the response list.


