ep_auth_session (samesite = none)
=============
Fork from [ep_auth_session](https://github.com/Kurounin/ep_auth_session) but sets the samesite property to none in the cookie.
A small script for [etherpad-lite](https://github.com/ether/etherpad-lite) which provides a route that authenticates the user with the provided sessionID parameter and redirects to the given padName.
Usefull when integrating etherpad in a application on a another domain.


## Install
[![ep_auth_session](https://nodei.co/npm/ep_auth_session_samesite_none.png)](https://www.npmjs.com/package/ep_auth_session_samesite_none)

Restart your etherpad-lite instance to recognize the plugin.

# Usage
Include an iframe with the src set to etherpad page /auth_session?sessionID=SESSION_ID&padName=PAD_NAME
```html
<iframe src="http://pad.test.de/auth_session?sessionID=SESSION_ID&padName=PAD_NAME" width="600" height="400"></iframe>
```
You can optionally include the groupID and lang as well
```html
<iframe src="http://pad.test.de/auth_session?sessionID=SESSION_ID&groupID=GROUP_ID&padName=PAD_NAME&lang=LANGUAGE" width="600" height="400"></iframe>
```
