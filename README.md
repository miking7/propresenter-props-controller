# propresenter-props-controller
The missing ProRemote **props layer controller**... implemented as a simple single-html-file SPA.  (Demo [here](http://resources.faithfm.com.au/proprops.html))

## The Motivation:

* The ProPresententer [ProRemote app](https://renewedvision.com/propresenter/mobile-apps/) is good for controlling many things, but surprisingly it doesn't let you control **prop layers**.
* The [ProPresenter Control](https://support.renewedvision.com/hc/en-us/articles/6032278869011-Using-ProPresenter-Control) web interface does let you control props, but is not practical to use on a **mobile device**.

This simple single-page app provides a mobile-friendly mechanism to enable/disable **prop layers** in ProPresenter from a **mobile device**.

![Screenshot 1](https://github.com/miking7/propresenter-props-controller/raw/main/screenshot-1.png)

## Usage Details:

* Make sure that ProPresenter's "Enable Network" option has been turned on (Network Settings), and note the IP address + port details found there.
* Click the settings gear icon in our proprops.html web page, and update the "address:port" to match the propresenter address details found in the previous step.
* An interface similiar to the screenshot above should be visible showing a button for each prop layer you have defined in ProPresenter.  
* Toggling these buttons will enable/disable the corresponding prop layer.
* As with any of ProPresenter's remote control options, rememeber that both devices need to be on the same network, and that ProPresenter's network API has been enabled.  
* For troubleshooting, a good step is to confirm you can access the ProPresenter Control web interface on http://server-ip:port/v1/control.

## Installation + Implementation:

To host this yourself, simply upload propremote.html to any web hosting platform.  (For demo purposes I've uploaded it [here](http://resources.faithfm.com.au/proprops.html), but I can't guarantee it will be hosted there indefinitely)

This web app uses the following resources:

* [Tailwind CSS](https://tailwindcss.com/)
* [Alpine JS](https://alpinejs.dev)
* [ProPresenter API](https://renewedvision.com/api_spec/index.html)
