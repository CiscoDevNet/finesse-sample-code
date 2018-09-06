# Cisco Finesse - Webex Teams Team Announcements Sample Gadget
The Webex Teams team announcements sample gadget demonstrates how to use the messaging capability of [Cisco Webex Teams](https://developer.webex.com) and the power of Finesse gadgets to make team communication easier and effective. This gadget leverages the Cisco Webex Teams API’s to easily post News, Notifications and Announcements to other team members (Agents / Supervisors) right from your Finesse Agent / Supervisor desktop. There is step-by-step instructions on how to add this gadget in your Finesse desktop.

![Sample Gadget Screenshot](Screenshot.png)

This sample gadget contains the following files:

	WebexTeamsTeamAnnouncements/
        bootstrap/
        images/
            Alert-ToggleOff-02.png
            Alert-ToggleOn-02.png
            Alert-ToggleOn.png
        oauth.html
		WebexTeamsTeamAnnouncements.css
		WebexTeamsTeamAnnouncements.js
		WebexTeamsTeamAnnouncements.xml
	WebexTeamsTeamAnnouncementSampleGadget.pdf

Download the version of the sample gadget that matches the Finesse version. Starting Finesse 11.0(1), sample gadgets will be forward compatible until compatibility is broken. At that time, a new version of the sample gadget will be published with the starting Finesse version number in the filename.

## Requirements
1. The sample gadget and the Finesse JavaScript library requires a deployment that includes Cisco Finesse. If you do not have a system that includes Cisco Finesse, you can reserve a [DevNet sandbox](https://developer.cisco.com/docs/finesse/#!sandbox) for developing your gadget.
1. Have Finesse system installed and configured.
1. Verify that you can login an agent into Finesse.
1. Ensure that you can have a Cisco Webex Teams account and can login. 

## Usage
1. Read the document WebexTeamsTeamAnnouncementSampleGadget.pdf for an overview about this sample gadget as well as step-by-step instructions on how to deploy the gadget.

## Additional Information
##### Finesse REST API
Documentation for the Finesse REST API can be found in the [Finesse Developer Guide](https://developer.cisco.com/docs/finesse/#!rest-api-dev-guide).

##### Finesse JavaScript Library
Documentation for the Finesse JavaScript library can be found on [DevNet](https://developer.cisco.com/docs/finesse/#!javascript-library) and is also located on the Finesse server at the following URL: http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/doc/index.html

- You can access the JavaScript library at the following URL (starting Finesse 10.6(1)): http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/finesse.js.

 If you have third-party gadgets, the third-party gadgets can access the JavaScript library at: /desktop/assets/js/finesse.js.

- You can access JQuery at the following URL (starting Finesse 10.6(1)): http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/jquery.min.js.

 If you have third-party gadgets, the third-party gadgets can access JQuery at: /desktop/assets/js/jquery.min.js.

**For proper functioning of the JavaScript library, you must import both the JavaScript library and JQuery.**

##### Cisco Webex Teams API
Documentation for the Cisco Webex Teams API can be found at [Cisco Webex for Developers](https://developer.webex.com).

## Disclaimer
This gadget is only a sample and is **NOT guaranteed to be bug free and production quality**.

The sample gadgets are meant to:
- Illustrate how to use the Finesse REST and JavaScript APIs
- Serve as an example of the step by step process of building a gadget using the Finesse JavaScript Library
- Provided as a guide for a developer to see how to initialize a gadget and set up handlers for user and dialog updates.

## Support Notice
[Support](https://developer.cisco.com/site/support) for the JavaScript library is provided on a "best effort" basis via DevNet. Like any custom deployment, it is the responsibility of the partner and/or customer to ensure that the customization works correctly and this includes ensuring that the Cisco Finesse JavaScript is properly integrated into 3rd party applications. Cisco reserves the right to make changes to the JavaScript code and corresponding API as part of the normal Cisco Finesse release cycle.

It is Cisco's intention to ensure JavaScript compatibility across versions as much as possible and Cisco will make every effort to clearly document any differences in the JavaScript across versions in the event that a backwards compatibility impacting change is made.

Cisco Systems, Inc.
[http://www.cisco.com](http://www.cisco.com)
[http://developer.cisco.com/site/finesse](http://developer.cisco.com/site/finesse)