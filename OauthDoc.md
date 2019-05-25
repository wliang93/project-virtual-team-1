## Useful Resources
* [Github Api]('https://developer.github.com/v3')
* [Github API-NewAuthorization](https://developer.github.com/v3/oauth_authorizations/#create-a-new-authorization)
* [Github - Building Oauth Apps]('https://developer.github.com/apps/building-oauth-apps/authorizing-oauth-apps/#non-web-application-flow')
* [Octonode]('https://github.com/pksunkara/octonode')
* [Electron Oath2 Tutorial]('https://medium.com/linagora-engineering/using-oauth-in-an-electron-application-abb0376c2ae0')

## Authentication Flow
1. Electron Auth2 is initialized in auth file
1. getUserInfo() -> is called by 
	* Generates an instance of client
1. The user visits new webpage to authorize this application
1. The user is redirected back to the application
	* The page will send back the token as a promise.
1. Electron app then has to store the token somewhere

## Setting up With Github
1. Application must be authorized with github, [here]('https://github.com/settings/applications/new')

## Misc Notes
* Owner may need to register Oauth tokens
* nodegit, and octonode used for github interfacing functions
