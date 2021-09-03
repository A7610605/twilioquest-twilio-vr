# A Helicopter Parent for Your Messages

For this objective, we'll ask you to set up [status callbacks](https://support.twilio.com/hc/en-us/articles/360008989454-Tracking-the-Delivery-Status-of-an-Outbound-Twilio-SMS-or-MMS-Message) for inbound messages using the `action` attribute of the `<Message>` tag ([docs](https://www.twilio.com/docs/sms/twiml/message#attributes-action)). Using your own web app, the **code editor**, or maybe a pair of [functions](https://www.twilio.com/console/functions/manage), you'll need to set up two routes/handlers - one [you'll use with your Twilio number](https://www.twilio.com/console/phone-numbers/<%= env.TQ_TWILIO_NUMBER_SID ? env.TQ_TWILIO_NUMBER_SID.value : '' %>) to respond to an incoming message, and another to receive status callbacks about the delivery status of your reply message.

In your status callback URL handler, print out the **message SID** and **status** of your outbound reply messages. Those are the values you will need to enter into the validation input fields on the right. Once you have your message SID and its final status, click the *HACK* button!