## Demid Efremov
## d.efremov@innopolis.university
## telegram: @Not_A_Snek
&nbsp;

## List and explain the key metrics used in SRE
As DevOps experts state, there are 5 key metrics in Software Reliability Engineering:

- Uptime - The portion of time the service is available for requests from users. Usually measured in % of month.

- Latency - The time it takes for a software to process a request. Usually measured in seconds or milliseconds.

- Traffic - Amount of demand put onto the service. Usually measured in requests/sec, concurrent sessions or KB/sec depending on service.

- Errors - The rate of service failing requests. Usually measured in % of requests failed.

- Saturation - Measure of utilization of the service resources. Usually measured in % of maximum utilization.


## Share the SLAs or reliability metrics you found for the two companies, along with any notable observations or insights

Google: At least 99.5% monthly uptime for most services. For services like Cloud SQL or Cloud DNS it is much higher, up to 100% monthly uptime. Google also incorporates discount system if uptime is less than expected, with rates as high as 50% for downtimes of 5% or higher.

Amazon: At least 99.9% monthly uptime for most services. For services Amazon Compute Service it is much higher, up to 99.99% monthly uptime. Just like Google incorporates discounts if SLA is not met. For some services discount is twice as low as Google's though.


## Discuss the importance of these metrics and how they contribute to the overall reliability and performance of software systems

For most remote (web) services there are two really important metrics - Uptime and Errors, as the show the overall reliability of service. Traffic and Saturation metrics show the performance of the service, and amount of concurrent events it can process. Latency meanwhile works as a metric for both performance and reliability, as high latency might show problems with both performance of the system or reliability of connection (or just bad internet client-side).
