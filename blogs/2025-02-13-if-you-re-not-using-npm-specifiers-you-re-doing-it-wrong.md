---
title: "If you're not using npm specifiers, you're doing it wrong"
url: "https://deno.com/blog/not-using-npm-specifiers-doing-it-wrong"
date: "2025-02-13T15:00:00.000Z"
author: "Andy Jiang"
feed_url: "https://deno.com/feed/"
---
One common way to import npm packages is with transpile services like esm.sh or unpkg.com, which converts npm modules to esm and hosts them on the web. However, since Deno 2, which supports npm natively, we recommend using npm specifiers. Here's why.
