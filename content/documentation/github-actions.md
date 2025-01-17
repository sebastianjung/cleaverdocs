---
title: 'GitHub Actions'
description: 'Integrate with GitHub Actions to use GHA as your dedicated build server.'
image: 'https://docs.cleavr.io/images/cleavr-twitter.png'
video: ''
---

Cleavr integrates with [GitHub Actions](https://github.com/features/actions), an automated workflow feature from GitHub, that allows 
you to perform several actions, such as building your app. 

<base-info>
GitHub allots up to 2,000 build minutes each month for free with additional paid-tiers available. 
</base-info>

Using Cleavr's GitHub Actions integrations allows you take advantage of GitHub's generous build-time to build your apps on GitHub 
instead of your own servers. This drastically frees up important resources on your server. 

**Best yet. Cleavr gets you started with no configuration required!**

When you enable the integration, Cleavr will automatically update your GitHub repository with a workflow that will build 
your app and adds a GitHub secret to keep your deployment hook private. 

## Available for the following app types
- Nuxt - Server Side Rendered (SSR)
- Nuxt - Static
- Adonis
- NodeJS - Server Side Rendered (SSR)
- NodeJS - Static

## Comparison
The following shows the difference in CPU Utilization on a server deploying the same app without the GitHub Actions integration 
compared to with the integration enabled. 

<img src="/images/deploy-compare.png" alt="comparison chart" />

You can see the time and memory utilization required to build the app on your own server is more than double. With GitHub 
Actions integration enabled, Cleavr merely waits for the build to be completed by GitHub and then downloads the resulting 
output files and then activates the deployment. 

## Advantages

**Dedicated build server** - having GitHub act as a build server frees up memory from your server, letting it be more 
stable for visitor traffic

**Run test scripts** - you can expand the workflow file run test automation 

**Add other steps** - if you're a GitHub Actions pro, flex your muscles

**Set up for multiple branches** - you can enable Actions just for Master, or for any other branch you'd like; 
each will have their own workflow file created

**Automatic deployments** - triggered when a change is committed to the branch being watched. 

## Enabling GitHub Actions

<base-info>
GitHub Actions is only available for projects on your GitHub account. This integration is not available for public repositories 
that are not your own. 
</base-info>

Navigate to the **Web App** you want to enable GitHub Actions for and then go to the **Settings** section. 

If you have not configured the settings for the web app, you will need to configure them first and click Update when completed. After 
the web app has been configured, then enabling the integration will be available on the **GitHub Actions** tab. 

Select the **GitHub Actions** switch to enable. 

![Enable GitHub Actions integration](/images/deployment/cleavr-node-enable-github-actions.png)


<base-alert>
Enabling the GitHub Actions integration will automatically trigger a deployment for the project / branch. 
</base-alert>

## Disabling GitHub Actions
You can disable the integration at any time from the GitHub Actions tab. If you disable, this will remove the secret key; 
however, the workflow files will remain.
