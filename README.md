# Quick Start

to compile the examples, issue the following command

`mvn compile`

To execute an example, run

`mvn exec:java -Dexec.mainClass="com.nexmo.messaging.sdk.examples.SendTextMessage"`

This will construct a message request and use the SDK to attempt to submit it.

The code can be seen in this class `src/main/java/com/nexmo/messaging/sdk/examples/SendTextMessage.java`

You can modify the constants at the top of the class to inject your own account credentials and message parameters.

    public static final String USERNAME = "account-id";
    public static final String PASSWORD = "password";

    public static final String SMS_FROM = "12345";
    public static final String SMS_TO = "447777111222";
    public static final String SMS_TEXT = "Hello World!";


`mvn exec:java -Dexec.mainClass="com.nexmo.messaging.sdk.examples.SendWapPush"` will execute an example wap-push submission.
The code can be found here `src/main/java/com/nexmo/messaging/sdk/examples/SendWapPush.java`
