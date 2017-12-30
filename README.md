# pals-reporting
Node app with exposed HTTP API endpoints for PALS' data processing tasks from CampMinder

High-Level Architecture:
* A backend service which exposes HTTP API endpoints to run each of the data processing tasks currently handled in Google App scripts
* Each task will talk to CampMinder and Google Sheets API to send / receive data
* A summary email with the results of the task will be sent to PALS staff or a dedicated reporting mailbox
* Schedule these tasks in an execution environment (e.g., Google Cloud Platform, AWS) to automate the process
