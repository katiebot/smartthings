# SmartThings SmartApps
## Electric Objects EO1
This SmartApp requires both an Electric Objects EO1 (while I don't have an EO2 to test with, I assume this will also work with the EO2 since there appears to only be one API) and a motion sensor already paired to your SmartThings.

When configuring the SmartApp, you need to define the following:
* Motion sensor
* Minutes to wait after motion sensor is inactive before turning the EO1 off
* EO1 device ID
* remember_user_token cookie from electricobjects.com (I haven't yet figured out how to handle authentication)

### EO1 device ID
This can be found by going to https://www.electricobjects.com/api/v6/user/devices/, the ID is the first item output on the page.

### remember_user_token cookie
This can be found by going to https://www.electricobjects.com/api/v6/user (or any electricobjects.com page while signed in) and using your browser developer tools to inspect cookies then copying and pasting the remember_user_token cookie.

---

### Credits
The motion sensor component was based on the example code in [this SmartApp tutorial](https://docs.smartthings.com/en/latest/getting-started/first-smartapp.html).
[This comment](https://github.com/harperreed/eo-python/issues/19#issuecomment-293348665) provided the necessary details for the Electric Objects API.
