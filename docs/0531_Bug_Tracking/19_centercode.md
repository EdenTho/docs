# Connect TestFairy to Centercode

## 1. Create a Centercode API Key

Open the Centercode Community Homepage, and go to Community Tools > Configuration > API Keys (under Advanced Configuration) > Create an API Key. Name the new API KEY "TestFairy".

![Create JIRA API](/img/bug-tracking/cenercode1.png)

![Set TEstFairy JIRA Key](/img/bug-tracking/centercode2.png)

## 2. Configure a Centercode extenrnal feedback source:

2.1 Click Project Tools
2.2 Click Feedback Types
2.3 Hover over your desired Feedback Type (Bug Reports) & click Modify
2.4 Click External Sources
2.5 Click "Create an External Source" 
2.6 From the External Sources creation page Create an (internally-facing) Name
2.7 Provide a simple Key to help identify this External Source  (ex: “appcrashlog” - detailed below)
2.8 Select the appropriate Workflow state (typically “New”)
2.9 Configure your Incoming Fields
2.10 Copy / Save your API Endpoint URL and click Submit

## 3. Configure a new webhook in your TestFairy settings: 

2.1. Open your TestFairy account Preferences 
