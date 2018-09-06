# Cisco Finesse - External REST API Sample Gadget
The external REST API sample gadget allows you to call an external REST API from the Finesse gadget. The response of the API request is printed on the gadget with no formatting. It is intended to serve as an example of how to call an external REST API using gadgets.io.makeRequest(). This sample illustrates how to format and pass in the necessary parameters for the gadgets.io.makeRequest().

![Sample Gadget Screenshot](Screenshot.png)

This sample gadget contains the following files:

	FinesseJavaScriptLibrary/
		readme.txt
	ExternalRestApi/
		ExternalRestApiSampleGadget.css
		ExternalRestApiSampleGadget.js
		ExternalRestApiSampleGadget.xml
	_readme.txt

Download the version of the sample gadget that matches the Finesse version. Starting Finesse 11.0(1), sample gadgets will be forward compatible until compatibility is broken. At that time, a new version of the sample gadget will be published with the starting Finesse version number in the filename.

## Requirements
1. The sample gadget and the Finesse JavaScript library requires a deployment that includes Cisco Finesse. If you do not have a system that includes Cisco Finesse, you can reserve a [DevNet sandbox](https://developer.cisco.com/docs/finesse/#!sandbox) for developing your gadget.
1. An external REST API to be called when a call arrives.

## Usage
1. Go to the handleNewDialog function and modify the variable url to the URL of the external REST API you want to call when a new call arrives.
2. Modify the "method" to the HTTP method of the external REST API.
3. If the external REST API requires a request body, uncomment the line of code that that sets the variable contentBody. Then, populate this variable with the content body of the external REST API. This variable is expected to be a string. So if the content body is a JSON object, make sure to convert it into a string.

 Also, uncomment the line of code that adds the contentBody to the options object as well as the line that adds the contentType. Then, modify the value of the contentType to the contentType of the external REST API.
4. If the external REST API requires an authorization header, uncomment the line of code that adds the authorization to the options object. If the authorization type is Basic Auth, then you can skip to the next step. If not, generate the authorization using the appropriate utility (not included) and change the authorization value to the one you generated.
5. Upload the sample gadget to the webserver.
6. Add the sample gadget to the desktop layout.
7. Log in the agent/supervisor and view the sample gadget.

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