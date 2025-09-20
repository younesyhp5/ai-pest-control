[Back to main page](README.md)

# AI Pest Control: Google products

## Search

### AI summaries

There is no setting to disable the feature.

You can add `-ai` to individual queries to turn off the AI summaries.

Firefox lets you change your search engine URL to always include this, YMMV: https://old.reddit.com/r/firefox/comments/1jei38p/made_a_firefox_extension_to_automatically_block/miissgw/

## Workspaces-wide

### "Ask Gemini" nag button in navbar

No setting to turn it off, but the buttons can be removed with JS (last tested 2025-09-20):

```js
document.querySelectorAll('button[aria-label="Ask Gemini"]').forEach(e => e.parentElement.parentElement.parentElement.remove())
```

## Drive

### "Ask Gemini" nag

The JS snipped for the other "Ask Gemini" nag feature actually removes this one too.

This one is particularly nasty because the page “self-heals” during certain user interactions.
So you will have to run it periodically.
