The queries shared in this section were created as reference examples for those who want to develop alerting and reporting mechanisms in Splunk. 

The SPL queries here are based on attack results that I personally conducted and tested.

The fields used in the queries (index, source, sourcetype, etc.) may vary depending on the type of logs being collected (Windows Event Log, syslog, etc.).

Some queries may require Data Models (e.g., Network_Traffic, etc.). To view these, you can run the `| datamodel` SPL command or check them by going to Settings -> Data Models in the interface.

Certain data models, such as `tstats`, may not work with comments containing "#". You may need to remove these comments. Also, commands like `tstats` may not work with time definitions like "Relative" (Last 30 minutes, Last 7 Days, etc.). It is recommended to use the "Date & Time Range" property.
