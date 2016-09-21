# Finesse Sample Code
This project contains sample gadgets and code to be used with [Cisco Finesse](http://developer.cisco.com/site/finesse), a next-generation agent desktop.

##### Finesse REST API
Documentation for the Finesse REST API can be found in the [Finesse Developer Guide](http://developer.cisco.com/site/finesse/docs/guides/rest-api-dev-guide).

##### Finesse JavaScript Library
Documentation Finesse JavaScript library can be found on [DevNet](http://developer.cisco.com/site/finesse/docs/guides/javascript-library) and is also located on the Finesse server at the following URL: http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/doc/index.html

- You can access the JavaScript library at the following URL (starting Finesse 10.6(1)): http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/finesse.js.

 If you have third-party gadgets loaded on Finesse, the third-party gadgets can access the JavaScript library at: /desktop/assets/js/finesse.js.
- You can access JQuery at the following URL (starting Finesse 10.6(1)): http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/jquery.min.js.

 If you have third-party gadgets loaded on Finesse, the third-party gadgets can access JQuery at: /desktop/assets/js/jquery.min.js.

**For proper functioning of the JavaScript library, you must import both the JavaScript library and JQuery.**

## Disclaimer
These gadgets are only a sample and are **NOT guaranteed to be bug free and production quality**.

The sample gadgets are meant to:
- Illustrate how to use the Finesse REST and JavaScript APIs
- Serve as an example of the step by step process of building a gadget using the Finesse JavaScript Library
- Provided as a guide for a developer to see how to initialize a gadget and set up handlers for user and dialog updates.

The Finesse JavaScript library and the sample gadgets are made available to Cisco partners and customers as a convenience to help minimize the cost of Cisco Finesse customizations. Cisco does not permit the use of this library in customer deployments that do not include Cisco Finesse.

## Support Notice
[Support](http://developer.cisco.com/site/devnet/support) for the JavaScript library is provided on a "best effort" basis via DevNet. Like any custom deployment, it is the responsibility of the partner and/or customer to ensure that the customization works correctly and this includes ensuring that the Cisco Finesse JavaScript is properly integrated into 3rd party applications. Cisco reserves the right to make changes to the JavaScript code and corresponding API as part of the normal Cisco Finesse release cycle.

It is Cisco's intention to ensure JavaScript compatibility across versions as much as possible and Cisco will make every effort to clearly document any differences in the JavaScript across versions in the event that a backwards compatibility impacting change is made.