[Back to main page](README.md)

# AI Pest Control: Google products

## Ads

You can turn personalized ads off under https://myadcenter.google.com/.

It's unclear if this affects data collection at all.

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

### General settings

Under settings https://drive.google.com/drive/settings

* Privacy: turn off “smart workspace settings”
* Manage apps: turn off Gemini

This is a good place to check that you turn off various data collection and other nonsense features.

### "Ask Gemini" nag

The JS snipped for the other "Ask Gemini" nag feature actually removes this one too.

This one is particularly nasty because the page “self-heals” during certain user interactions.
So you will have to run it periodically.

## Youtube

There doesn't seem to be any AI-related settings on Youtube. Personalization/data collection is handled via the Google settings.

### For creators: third-party training

There is an opt-in setting in **Youtube Studio** -> **Settings** -> **Channel** -> **Advanced settings** -> **Third-party training** -> **Allow third-party companies to train AI models using my channel content (off)**.

It's not clear how to make sure first-party companies (i.e., Alphabet/Google) from training on your stuff.
