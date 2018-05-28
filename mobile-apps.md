Using a modified Android app, you can regain access to Google Maps search and voice search!
As of now, there is no modified iOS app available. :(

## Using a modified Android .apk

First of all, massive thanks to [/u/navdyh4x0r](https://www.reddit.com/user/navdyh4x0r)'s [fantastic post](https://np.reddit.com/r/navdy/comments/84o0gt/working_search_on_android/) outlining what was needed to replace the Google Maps API keys!

Thanks to that, [/u/coronafire](https://www.reddit.com/user/coronafire) made [another excellent post](https://www.reddit.com/r/navdy/comments/8eilgy/working_search_and_maps_on_android/) where he rebuilt the .apk with his own personal API key for Google and HERE.  He also did some [substantial work](https://gitlab.com/alelec/navdy/android-navdy-client/commit/a5cc31b874f461cb6ef5a11526a6113fad77e5bb) to replace all usage of the Google Maps for Business API.  He goes into detail about the changes he made, and his code is open-sourced on GitLab: [android-navdy-client](https://gitlab.com/alelec/navdy/android-navdy-client)!  I highly recommend you read his post and use the current builds he provided at the end!

## Instructions

1. Download .apk from above source
2. Uninstall existing Navdy app (this step was necessary for me, but you can try to skip it first)
3. Copy .apk to your phone, allow installation from unknown sources, and run the .apk to install
