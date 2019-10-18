# MicrosoftFlowAzureFunction

This function provides a REST interface to Blue Prism Processes. It allows invocation from the Blue Prism Connector for Microsoft Flow.
This may also be useful for those who need a generic REST interface to Blue Prism, which currently only supports SOAP.

Simple name value pairs are supported, but not complex objects/collections.

A JSON payload like this:

`{
  "CustomerName" : "Mike Jones",
  "AccountNumber" : "12345"
}`

Is automatically transfomed to SOAP/XML like this:

`<xml>
  <CustomerName>Mike Jones</CustomerName>
  <AccountNumber>12345</AccountNumber>
</xml>`
