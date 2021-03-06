# StreamMarker

[StreamMarker](https://www.streammarker.com/) is a complete system for measuring, recording, and viewing environment readings. These currently consist of:
 * Soil Temperature
 * Soil Moisture
 * Atmospheric Temperature
 * Atmospheric Humidity
 * Sensor Enclosure Temperature

The following components have been published as Open-Source:
 * [streammarker-web](https://github.com/skidder/streammarker-web) - Web Dashboard for viewing measurements and managing sensors & relays
 * [streammarker-data-access](https://github.com/skidder/streammarker-data-access) - REST endpoint to query for sensor readings and manage sensors & relays
 * [streammarker-collector](https://github.com/skidder/streammarker-collector) - REST endpoint to receive sensor readings sent by relay devices and enqueue messages on SQS for asynchronous processing
 * [streammarker-writer](https://github.com/skidder/streammarker-writer) - SQS consumer that records sensor readings to DynamoDB
