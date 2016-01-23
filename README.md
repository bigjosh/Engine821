# Engine821

Engine821.com is a system that lets you process incoming email with custom java code.

It is different from the many other systems out there becuase...

1. It lets you take part in every step of the SMTP state machine. 
2. It has a very clean and simple design. 
3. It is actively maintained by people who care about reliability and correctness.

To use the service, you create two classes...

* `MessageHandlerFactory`
* `MessageHandler`
 
...and upload these to the Engine821.com system. Then you configure what domains and subdomains you want to go to your `MessageHandler` set. After that, each time a new message comes in, we call your code with each of the steps in the receiving process.

