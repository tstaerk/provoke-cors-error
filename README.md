# provoke-cors-error
The idea is to load e.g. stock prices from public websites into a database.

However, javascript code to load a website ("load a website from a website") results in a CORS error, here I reproduce it.

However, when I do it in https://github.com/tstaerk/chrome-extensions it works.
https://github.com/tstaerk/chrome-extensions uses await fetch(
      `https://translate.googleapis.com/translate_a/single?client=gtx&sl=auto&tl=de&dt=t&q=${encodeURIComponent(
        text
      )
  to fetch via https.
