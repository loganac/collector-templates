# Box REST Collector

This collector template allows you to collect logs from Box.

# Creating the Client Grant Credentials

You will need an admin or have access to create credentails within your organizations Developer Console. This can typically be found using your organizations URL app.box.com/developers/console.

1) Login to your Organization Box Developer Console
2) From the Console, fine the `Create Platform App` button in blue in the top right corner of the page
3) Select Custom App
4) Add your details to the `Create a Custom App` -> "App Name", "Description (Optional)", "Purpose", "Who is building this application? (Optional)". Then click, `Next`
5) Select the `Server Authentication (Client Credentialas Grant)`
6) Click `Create App`
7) For `App Access Level` be sure to select "App + Enterprise Access"
8) Under `Application Scopes` be sure to select the following: "Manage Enterprise Properties" - This is the endpoint for collecting `Events`. For Users and Groups, add the "Manage users" and "Manage groups". You can select/de-select these options later.
9) To create you API token, locate the `Advanced Features`, check the `Generate user access tokens` box.
10) Save your changes
11) Depending on your organization, you will need to `Review and Submit` for approval of the app creation. You will need to login to you Box Admin console to approve the newly created app.
12) On the Box Admin Console, navigate to the `Integrations` menu
13) Select the `Platform Apps Manager`, then select the `Platform App Manager` tab.
14) Locate your app and approve using the `More` option or the three dots option. You will also need to enable the app for the API requests to run.




# Installation

1) Copy the contents of breaker.json
2) Navigate to Event Breaker Rules under Processing -> Knowledge
3) Create a new breaker ruleset
4) Edit as JSON and paste the previously copied JSON into place; save
5) Copy the contents of collector.json
6) Navigate to Data -> Sources -> REST Collectors
7) Add Collector
8) Configure as JSON tab (at the top of the window)
9) Paste the JSON from collector into the screen and save
10) If there are fields for you to fill out, you will be prompted here. When done, hit Replace variables.
12) Commit and Deploy


### Event Breaker

Use the included breaker.json file as above

## Author
Unknown User - unknown@cribl.io
