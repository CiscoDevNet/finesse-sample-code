# Cisco Finesse - CUIC Sample Gadget
The CUIC sample gadget demonstrates how to create a gadget that displays a permalink in an iframe. The gadget is rendered whenever the tab the gadget is on is first visible. It is intended to serve as an example of placing a CUIC permalink in a Finesse gadget. This sample illustrates how to initialize the gadget, and to set up a handler for determining when the tab that that gadget is on is visible.

This sample gadget is applicable to CUIC 11.6(1) and below. For CUIC 11.6(2) and above, use the out of the box CUIC gadget (LiveDataGadget.jsp or HistoricalGadget.jsp) to embed CUIC reports in Finesse. Please see the ***Unified Intelligence Center Gadgets in Cisco Finesse*** section of the [***Cisco Unified Intelligence Center User Guide***](https://www.cisco.com/c/en/us/support/customer-collaboration/unified-intelligence-center/products-user-guide-list.html) for more details.

![Sample Gadget Screenshot](Screenshot.png)

This sample gadget contains the following files:

	CUIC/
		CUIC.css
		CUIC.js
		CUIC.xml
    FinesseJavaScriptLibrary/
		readme.txt
	_readme.txt
	CUIC Finesse gadget.pdf

Download the version of the sample gadget that matches the Finesse version. Starting Finesse 11.0(1), sample gadgets will be forward compatible until compatibility is broken. At that time, a new version of the sample gadget will be published with the starting Finesse version number in the filename.

## Requirements
1. You must be using CUIC 11.6(1) or below.
1. The sample gadget and the Finesse JavaScript library requires a deployment that includes Cisco Finesse. If you do not have a system that includes Cisco Finesse, you can reserve a [DevNet sandbox](https://developer.cisco.com/docs/finesse/#!sandbox) for developing your gadget.
1. CUIC installed.
1. A permalink from a CUIC report. You must manually replace & to `&amp;` in the url.

## Usage
1. Read the document CUIC Finesse gadget.pdf for an overview about this sample gadget as well as instructions on how to modify the permalink and upload your gadget.
2. Make sure you manually replace & to `&amp;` in the url.

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

## Disclaimer
This gadget is only a sample and is **NOT guaranteed to be bug free and production quality**.

The sample gadgets are meant to:
- Illustrate how to use the Finesse REST and JavaScript APIs
- Serve as an example of the step by step process of building a gadget using the Finesse JavaScript Library
- Provided as a guide for a developer to see how to initialize a gadget and set up handlers for user and dialog updates.

## Support Notice
[Support](https://developer.cisco.com/site/support) for the JavaScript library is provided on a "best effort" basis via DevNet. Like any custom deployment, it is the responsibility of the partner and/or customer to ensure that the customization works correctly and this includes ensuring that the Cisco Finesse JavaScript is properly integrated into 3rd party applications. Cisco reserves the right to make changes to the JavaScript code and corresponding API as part of the normal Cisco Finesse release cycle.

It is Cisco's intention to ensure JavaScript compatibility across versions as much as possible and Cisco will make every effort to clearly document any differences in the JavaScript across versions in the event that a backwards compatibility impacting change is made.

Cisco Systems, Inc.<br>
[http://www.cisco.com](http://www.cisco.com)<br>
[http://developer.cisco.com/site/finesse](http://developer.cisco.com/site/finesse)