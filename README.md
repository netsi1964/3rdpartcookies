# 3rdpartycookies version 0.1
An iframe you can add to your page and know if 3rd part cookies are blocked on your page

## How to use
For now you can use it by adding an iframe like this:

```
<iframe src="https://3rdpartycookies.netlify.app/"></iframe>
```

You can the listen for a message to get information about if it was possible to set a cookie in the iframd.
In the [test](https://3rdpartycookies.netlify.app/test.html) I do this:

```
window.addEventListener("message", (event) => {
  const info = event.data;
  document.querySelector('#info').textContent = 
    `Received this info from iframe: ${JSON.stringify(info, null, 2)}`
}, false);
```

## Demo

You can see at test here: [test](https://3rdpartycookies.netlify.app/test.html)

## Feedback
Feedback is welcome. Create an [issue](https://github.com/netsi1964/3rdpartycookies/issues) and I will look into it.

I am also on Twitter where you can [tweet to netsi1964](https://twitter.com/netsi1964).

(c) 2021 [netsi1964](https://twitter.com/netsi1964).