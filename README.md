# redirect_url

https://stackoverflow.com/questions/503093/how-do-i-redirect-to-another-webpage

jQuery is not necessary, and `window.location.replace(...)` will best simulate an HTTP redirect.

`window.location.replace(...)` is better than using `window.location.href`, because `replace()` does not keep the originating page in the session history, meaning the user won't get stuck in a never-ending back-button fiasco.
