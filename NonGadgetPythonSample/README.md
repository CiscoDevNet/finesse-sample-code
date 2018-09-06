# Cisco Finesse - Non-Gadget Python Sample
The non-gadget Python sample presents a Python script that utilizes the Finesse REST APIs to sign in/out, change the agent state, and do a GET on the user. The example script implements the logic to connect to the Finesse Notification Service using the [SleekXMPP Library](http://sleekxmpp.com/) to receive Finesse notifications. Other [Python XMPP libraries](http://xmpp.org/software/libraries.html) are also available. All responses and events will simply print to the console. This script does NOT integrate these Finesse notifications back to the User object. This code has been tested with Finesse 11.5 and Python 3.4.2.

This sample contains the following files:

    finesse.py
    PythonSample.pdf

## Requirements
1. The sample gadget and the Finesse JavaScript library requires a deployment that includes Cisco Finesse. If you do not have a system that includes Cisco Finesse, you can reserve a [DevNet sandbox](https://developer.cisco.com/docs/finesse/#!sandbox) for developing your gadget.
1. [requests](http://docs.python-requests.org): This script requires the requests library to be installed and imported. This library is used to make the Finesse REST API requests. Please see the Usage section for installation instructions.
1. [XMPP Library](http://xmpp.org/software/libraries.html): [SleekXMPP](http://sleekxmpp.com) is the XMPP library used to connect to the Notification Service to receive events. The python script depends on the library be installed and imported. Developers can have a choice of using this library or utilizing their own. Please see the Usage section for installation instructions.

## Usage
In order to run this Finesse Python script, you will need to install Python, the Requests library, and the SleekXMPP library.

1. Install Python
 * Install Python 3.4.2 or above for your operating system.
 * Download the installer here: [https://www.python.org/downloads](https://www.python.org/downloads)
2. Install the Requests Library
 * Learn about the [Requests Library](http://docs.python-requests.org)
 * To install Requests for Python 3 on Mac OS, use these command line commands:
<pre><code>sudo curl -O https://bootstrap.pypa.io/get-pip.py
sudo python3 get-pip.py
pip3 install requests</code></pre>
 * To install Requests on Windows:
     * Pip comes with Python 3.4 Windows
     * Check to see if Pip is in your python 3 path:
<pre><code>C:\>pip –V
pip 1.5.6 from C:\Python34\lib\site-packages</code></pre>
     * If pip is in the Python34 path, the execute
<pre><code>pip install requests</code></pre>
3. Install SleekXMPP
 * Learn about the [SleekXMPP Library](http://sleekxmpp.com)
 * To install SleekXMPP, execute this command line command:
<pre><code>pip3 install sleekxmpp</code></pre>
4. Run the Finesse Python Script
 * Execute this command line command on MacOS:
<pre><code>python3 finesse.py</code></pre>
 * Execute this command line command on Windows:
<pre><code>py –3 finesse.py</pre></code>
or
<pre><code>python finesse.py</code></pre>

## Additional Information
##### Finesse REST API
Documentation for the Finesse REST API can be found in the [Finesse Developer Guide](https://developer.cisco.com/docs/finesse/#!rest-api-dev-guide).

## Disclaimer
This sample code is only a sample and is **NOT guaranteed to be bug free and production quality**.

The sample code is meant to:
- Serve as an example of the step by step process of writing a python script using the Finesse REST APIs.
- Provided as a guide for a developer to see how to use a Python XMPP library to process the Finesse notifications.

## Support Notice
[Support](https://developer.cisco.com/site/support/) for the sample code is provided on a "best effort" basis via DevNet. Like any custom deployment, it is the responsibility of the partner and/or customer to ensure that the customization works correctly and this includes ensuring that the sample code is properly integrated into 3rd party applications.

Cisco Systems, Inc.<br>
[http://www.cisco.com](http://www.cisco.com)<br>
[http://developer.cisco.com/site/finesse](http://developer.cisco.com/site/finesse)