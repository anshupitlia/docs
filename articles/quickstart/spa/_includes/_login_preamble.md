## Add Authentication with Auth0

The [Auth0 hosted login page](/hosted-pages/login) is the easiest way to set up authentication in your application. We recommend using the Auth0 hosted login page for the best experience, best security and the fullest array of features. This guide will use it to provide a way for your users to log in to your ${library} application.

::: note
You can also embed the Lock widget directly in your application. If you use this method, some features, such as single sign-on, will not be accessible. 
<% if (typeof embeddedLoginLink == 'string') { %>
To learn how to embed the Lock widget in your application, follow the [Embedded Login sample](${embeddedLoginLink}).
<% } %>
:::

When a user logs in, Auth0 returns three items:
* `access_token`: an access token. To learn more, see the [access token documentation](/tokens/access-token).
* `id_token`: an ID token. To learn more, see the [ID token documentation](/tokens/id-token).
* `expires_in`: the number of seconds before the access token expires

You can use these items in your application to set up and manage authentication. 
