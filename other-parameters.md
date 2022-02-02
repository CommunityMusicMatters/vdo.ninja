# Other Parameters

There are some more parameters on [VDO.Ninja](https://vdo.ninja) which are currently not ready for production, not intended to be used, or not well-documented.

| Parameter           | Explanation                                                                                                                                                                                                                                                                                  |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `&aspectratio`      | changes the aspect ratio on the publisher side. Floating point value; 1.777777 is common. not supported by all browsers.                                                                                                                                                                     |
| `&crop`             | <p>changes the aspect ratio on the publisher side, but lets you pass an integer value to represent a percentile cropping value. <br><br>So, &#x26;crop=10 will reduce the aspect ratio by 10% and &#x26;crop=-10 will increase the aspect ratio.  The assumed base aspect ratio is 16:9.</p> |
| `&debug`            | Sends live debug log data to a remote server. That debug server is normally off, but this flag can be used by Steve to debug issues remotely. The debug data is not stored at any point.                                                                                                     |
| `&directorview`     | not currently an active feature                                                                                                                                                                                                                                                              |
| `&forceaspectratio` | not currently an active feature                                                                                                                                                                                                                                                              |
| `&layout`           | Takes a JSON string representing how the video mixer should arrange video elements. The string needed is based on the vdo.ninja/mixer app's layout structure.  Mainly used for development testing.                                                                                          |
| `&nomouseevents`    | Disables 'some' of the mouse/touch/drag triggers and events.  for debugging and niche situations.                                                                                                                                                                                            |
| `&nonacks`          | <p>'tries' to force the browser to not send keyframes or lower quality/resolution. doesn't really work.<br><br>tells the browser to not send NACK feedback</p>                                                                                                                               |
| `&nopli`            | <p>tries to find ways to combat frame stutter caused by packet loss or keyframe requests. Doesn't really work.<br><br>tells the browser to not send picture loss indicators</p>                                                                                                              |
| `&noremb`           | deletes the flag for Chrome's bandwidth estimation logic                                                                                                                                                                                                                                     |
| `&retry`            | used in rare cases, sometimes with the Raspberry Ninja project, where the peer connection may "crash" and the remote viewer won't bother to try reconnecting                                                                                                                                 |
| `&retrytimeout`     | should not be changed. value in milliseconds                                                                                                                                                                                                                                                 |
| `&slot`             | not currently an active feature                                                                                                                                                                                                                                                              |
| `&speedtest`        | forces essentially UDP mode, unless TCP is specified, and some other stuff                                                                                                                                                                                                                   |
| `&viewereffect`     | not currently an active feature                                                                                                                                                                                                                                                              |
| `&wss`              | specify the handshake server address to use                                                                                                                                                                                                                                                  |

There is a Google Sheet of all parameters available:\
[https://docs.google.com/spreadsheets/d/1rNPus\_c6fLwNIKOr1WCZZVMRWtlNJttUNtvvelInuRU/edit#gid=1565581695](https://docs.google.com/spreadsheets/d/1rNPus\_c6fLwNIKOr1WCZZVMRWtlNJttUNtvvelInuRU/edit#gid=1565581695)