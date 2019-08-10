---
id: secrets
title: Secrets
---

Unubo allows you to create environment variables by using Secrets. Secrets are encrypted and are only available to your app.

## Adding secrets to your app
Go to `Overview` page of your app, then expand the `Secrets` section to add a new secret.
<br/>
Once deployed, secrets are made available to your application as environment variables.
<br/><br/>
For example, this is how you would access a secret with a name of `DATABASE_URL` in Node.js.

```javascript
const DATABASE_URL = process.env.DATABASE_URL;
```