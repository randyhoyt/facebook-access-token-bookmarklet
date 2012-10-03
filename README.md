Facebook has a tool that generates *short-lived* access tokens for all your apps, but it's not as easy as you might think to get a *long-lived* token manually. This bookmarklet bridges that gap.

1. Drag this link to the Bookmarks bar in your browser: <a href="javascript: access_token=encodeURIComponent(window.getSelection());if(!access_token) void(access_token=prompt('Access Token: '));void(app_id=prompt('App ID: '));void(app_secret=prompt('App Secret: '));location.href='https://graph.facebook.com/oauth/access_token?client_id='+app_id+'&client_secret='+app_secret+'&grant_type=fb_exchange_token&fb_exchange_token='+access_token;">Get Access Token</a>.
1. Have your Facebook App ID and App Secret handy.
1. Visit the Facebook Access Token Tool in your browser to get short-lived tokens.
1. Select/highlight the short-lived token you want to convert into a long-lived token. (Double-clicking on the token should select it.)
1. Click the bookmarklet and specify values in the two prompts:
    1. App ID
    1. App Secret
1. The browser will load a Facebook response with the long-lived token in it. It will be the long string after the <code>access_token=</code> and before the <code>&expires</code>.