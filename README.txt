This plugin monitors forums (via TapaTalk API) for activity.

Following configuration parameters can be used to alter behavior at runtime

Parameter      (default) - description
pollInterval   (60)      - Interval at which the check for activity (s)
postChannel    ("")      - Channel to post updates to
watchedThreads ("")      - whitespace separated list of thread IDs to follow
                           ID form is [FORUM]:[THREADID]

If either postChannel or watchedThreads is empty monitoring is effectively disabled.

This plugin uses Tapatalk API for communicating with the Forum.

https://tapatalk.com/api.php

Only get_thread method is currenrly used and implementation should be compatible with
API versions 3 and 4.

The forums need to be configured in plugin.py (this will likely change later).

