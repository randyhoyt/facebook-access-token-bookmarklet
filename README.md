Facebook has a tool that generates *short-lived* access tokens for all your apps, but it's not as easy as you might think to get a *long-lived* token manually. This bookmarklet bridges that gap.

1. Visit the <a href="https://dl.dropbox.com/u/82944/facebook-access-token-bookmarklet.html" target="_blank">Bookmarklet Installation Page</a> and drag the link there to the Bookmarks bar in your browser.
1. Have your Facebook App ID and App Secret handy.
1. Login to the <a href="https://developers.facebook.com/tools/access_token/" target="_blank">Facebook Access Token Tool</a> in your browser to see short-lived tokens for all your apps.
1. Select/highlight the short-lived token you want to convert into a long-lived token. (Double-clicking on the token should select it.)
1. Click the bookmarklet and specify these values (which you should have handy) in the two prompts:
    1. App ID
    1. App Secret
1. The browser will load a Facebook response with the long-lived token included in it. It will be the long string after the <code>access_token=</code> and before the <code>&expires</code>.