---
id: express
title: Deploy Node Express app
sidebar_label: Express
---

You can deploy a Node Express app to Unubo in a few steps.

## Example app

<a href="https://github.com/unubo/express-on-unubo-cloud" target="_blank">Express on Unubo</a>

## Create an app

Go to the <a href="https://unubo.app/apps/new" target="_blank">New apps</a> page and select Node.js from the Apps section to get started.
<br/>
Choose a name and region for your app. Visit the [Regions](getting-started/regions.md) page to understand about choosing regions.

## Preparing your app

All apps on Unubo run on various ports. Use the "PORT" environment variable to allow Unubo to set the port for your app.
<br/>

```javascript
const PORT = process.env.PORT || 3000;
```

## Choose repo

Connect your GitHub account and choose which repo you want to deploy from.
<br/>
Visit the [Connect to GitHub](getting-started/github.md) page to learn about managing repo access.

## Commands

Add the following command in the commands list.

| Command   |
| --------- |
| npm start |

Note that by default Unubo adds the `npm install --production` command. This command does not install dev dependencies of your app.
If you need to install dev dependencies, add `npm install` to the list of commands.

## Deploy

Select the "Deploy" button to deploy your app to Unubo. Once the build process is complete, your app will now be live.
<br/>
Unubo creates a unique URL based on the name of your app `https://your-app-name.unubo.app`.
<br/><br/>
<a href="https://express.unubo.app" target="_blank">https://express.unubo.app</a>

## Related docs

[Check the status of your app](getting-started/status-monitor.md)
<br/>
[Add environment variables with secrets](getting-started/secrets.md)
<br/>
[Check your app's logs](getting-started/logs.md)
<br/>
[Rollback a deployment](getting-started/deployment-history.md)
<br/>
[Adding a custom domain](getting-started/domains.md)
