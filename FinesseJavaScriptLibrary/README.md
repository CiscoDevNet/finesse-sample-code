# Cisco Finesse JavaScript Library
### Documentation
Documentation for the Finesse JavaScript library can be found on [DevNet](https://developer.cisco.com/docs/finesse/#!javascript-library). Starting with Finesse 10.6(1), it is also located on the Finesse server at the following URL: http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/doc/index.html

## Requirements
This library depends on and requires the following objects to be present:
- gadgets.* APIs (specifically gadgets.json, gadgets.io and gadgets.Hub)
- jQuery

## Usage
The gadgets.* APIs are generally provided by the gadget container for gadget code to invoke. Certain APIs may only be available if specified as a "required feature" in the gadget specification XML; gadgets.json and gadgets.io are provided while gadgets.Hub requires the "pubsub2" feature specified in the &lt;ModulePrefs&gt; node:
```xml
<ModulePrefs>
    ...
    <Require feature="pubsub-2" />
    ...
</ModulePrefs>
```

Starting with Finesse 10.0(1), gadgets must also specify the "setprefs" feature in the &lt;ModulePrefs&gt; node. Developers will also want to import the Finesse Javascript Library (finesse.js) prior to accessing the "authorization" property from the gadget prefs.

Starting with Finesse 10.6(1), jQuery and the Finesse JavaScript library can be accessed from the Finesse server at the following URL: http(s)://&lt;FQDN&gt;:&lt;port&gt;/desktop/assets/js/finesse.js.

For third-party gadgets, the following imports can be used:
```xml
<!-- jQuery -->
<script type="text/javascript" src="/desktop/assets/js/jquery.min.js"></script>

<!-- Finesse Library -->
<script type="text/javascript" src="/desktop/assets/js/finesse.js"></script>
```

Usage of the finesse.restservices classes simply require ClientServices to be initialized:

```javascript
finesse.clientservices.ClientServices.init(obj);
```

Please refer to the documentation for the specific parameters required by this method, and to the sample gadget code for how to obtain this information.

**For proper functioning of the JavaScript library, you must import both the JavaScript library and JQuery.**

## Disclaimer
The Finesse JavaScript library and the sample gadget are made available to Cisco partners and customers as a convenience to help minimize the cost of Cisco Finesse customizations. Cisco does not permit the use of this library in customer deployments that do not include Cisco Finesse.

## Support Notice
[Support](https://developer.cisco.com/site/support) for the JavaScript library is provided on a "best effort" basis via DevNet. Like any custom deployment, it is the responsibility of the partner and/or customer to ensure that the customization works correctly and this includes ensuring that the Cisco Finesse JavaScript is properly integrated into 3rd party applications. Cisco reserves the right to make changes to the JavaScript code and corresponding API as part of the normal Cisco Finesse release cycle.

It is Cisco's intention to ensure JavaScript compatibility across versions as much as possible and Cisco will make every effort to clearly document any differences in the JavaScript across versions in the event that a backwards compatibility impacting change is made.

Cisco Systems, Inc.<br>
[http://www.cisco.com](http://www.cisco.com)<br>
[http://developer.cisco.com/site/finesse](http://developer.cisco.com/site/finesse)