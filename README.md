# Splunk Windows Event Log Home Lab

This lab explores monitoring logon and credential manager events using Splunk Enterprise on a Windows host. It accompanies the lab walkthrough video on YouTube.

## Walkthrough Video

Watch the full lab walkthrough on YouTube: [Windows Event Log Home Lab Walkthrough](https://www.youtube.com/watch?v=3CiRs6WaWaU&list=PLlIr0D2kbUZODythCTlQ0JMbO8bigYO6P&index=10).

## Tools Used

- **Splunk Enterprise (Windows)** – installed locally on a Windows host to ingest Windows Event Logs.
- **Windows Event Viewer** – to generate test events and confirm logs.
- **Web browser** – to interact with the Splunk web interface and create searches and dashboards.

## Example SPL Search

```
host="Dakotah-DT" source="WinEventLog:Security" "EventCode=5379"
```

This search filters Security logs on host `Dakotah-DT` for EventCode 5379 and is used to populate the dashboard table.

## Windows Event Log Inputs

The lab indexes the following Windows log channels from the host:

- **Application**
- **Security**
- **System**

## What I Practiced

- Installing Splunk Enterprise and setting up Windows Event Log inputs.
- Configuring a local event log collection input and selecting the correct channels.
- Verifying that events are being ingested by running searches in Splunk.
- Narrowing searches by host, source, sourcetype and EventCode.
- Creating a table view of search results and adding it to a dashboard.
- Building a basic dashboard panel and setting it as the home dashboard in Splunk.

## Screenshot evidence captured

| Step | Evidence |
|---|---|
| Splunk installation | ![Splunk installation](Splunk%20Download.png) |
| Select Windows Event Log inputs | ![Select Windows Event Log inputs](Selecting%20inputs.png) |
| Local event log input configured | ![Local event log input configured](Local%20event%20log.png) |
| Data input menu | ![Data input menu](Data%20Input.png) |
| Confirm logs are searchable | ![Confirm logs are searchable](Confirming%20logs%20are%20working.png) |
| Narrow search results | ![Narrow search results](Narrowing%20down%20the%20search.png) |
| Create table view | ![Create table view](Created%20Table%20view%20of%20search%20.png) |
| Create dashboard | ![Create dashboard](Creating%20a%20dashboard.png) |
| Add table chart | ![Add table chart](Adding%20a%20table%20chart.png) |
| Add customized search to table | ![Add customized search to table](Adding%20customized%20search%20for%20table.png) |
| Set dashboard as main dashboard | ![Set dashboard as main dashboard](Setting%20dashboard%20as%20main%20dash%20on%20home.png) |
