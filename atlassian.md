
[Back to main page](README.md)

# AI Pest Control: Atlassian products

## Platform-wide

### Rovo Chat nags

There is no setting to disable the feature.

You can at least take out the two buttons with Javascript:

```js
document.querySelector('[data-testid="app-navigation-ai-mate"]').remove() // takes out the "Rovo Chat" button in the navbar
document.querySelector('[data-testid="platform-ai-button"]').parentElement.remove() // takes out the button in the bottom right
```

## Jira

### Pre-written reply suggestions

Go to Jira settings and disable “Smart replies in work item comments”.
