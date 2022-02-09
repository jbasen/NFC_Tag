This module allows NFC tags read by a smart phone to trigger
smart home automations.  The module requires http messages to
be sent to it from an NFC reader (typically and iPhone or an
Android phone) in the format

http://[Processor IP]:[Processor Port]/?tag=[Tag ID]&secret=[Security Key] 

The Shortcut app on an iPhone or Tasker app on an Andriod phone
can be used to generate the above http GET request when an NFC
Tag is read.  On an iPhone this is setup as follows:

1.	Open the Shortcut app
2.	Select "Automation" from the menu bar on the bottom of the screen
3.	Press the "+" button in the upper right hand corner of the screen
4.	Press the button labeled "Create Personal Automation"
5.	Scroll down and select "NFC Ex. "When I tap an NFC Tag""
6.	Select "NFC Tag Scan"
7.	Scan your NFC tag by holding the phone next to it
8.	Enter a name for your NFC tag
9.	Press the "Next" button in the upper right hand corner of the screen

At this point you are ready to create the linkage between the act 
of scanning your NFC tag and the rest of your smart home.  To create 
the linkage:

1.	Press the "Add Action" button
2.	From the categories of actions choose "Web"
3.	Scroll down and from the list of items under "Web Requests" choose "Get Contents of URL"
4.	Enter an URL in the following format:

http://[Processor IP Address]:[Processor Port]/?tag=[Name for Tag Action]&secret=[Secret Key]
