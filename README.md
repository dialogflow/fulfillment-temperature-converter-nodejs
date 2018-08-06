# Temperature Trivia

## Setup
Select **only one** of three options below.

### Option 1: Add to Dialogflow (recommended)
Select [![Temperature Trivia](https://storage.googleapis.com/dialogflow-oneclick/deploy.svg "Temperature Trivia")](https://console.dialogflow.com/api-client/oneclick?templateUrl=https%3A%2F%2Fstorage.googleapis.com%2Fdialogflow-oneclick%2Ftemperature-converter-agent.zip&agentName=TemperatureConverterSample) to create a new agent.

### Option 2: Dialogflow Inline Editor
1. Create a [Dialogflow Agent](https://console.dialogflow.com/).
2. `git clone https://github.com/dialogflow/fulfillment-temperature-converter-nodejs.git`
3. Go to **Settings** ⚙ > **Export and Import** > **Restore from zip** using the `dialogflow-agent.zip` in this directory.<sup>A.</sup>
4. **Fulfillment** > **Enable** the [Inline Editor](https://dialogflow.com/docs/fulfillment#cloud_functions_for_firebase)<sup>B.</sup>
5. Under **Fulfillment** > **Inline Editor** > copy the code from this repo in `functions/index.js` and paste into the `index.js` file.
6. Under **Fulfillment** > **Inline Editor** > add `"dialogflow-fulfillment": "^0.5.0"` to the `package.json` file's `dependencies` object.
7. Select **Deploy**.

### Option 3: Firebase CLI
1. Create a [Dialogflow Agent](https://console.dialogflow.com/).
2. `git clone https://github.com/dialogflow/fulfillment-temperature-converter-nodejs.git`
3. Go to **Settings** ⚙ > **Export and Import** > **Restore from zip** using the `dialogflow-agent.zip` in this directory.<sup>A.</sup>
4. `cd` to the `functions` directory
5. Run `npm install`
6. Install the Firebase CLI by running `npm install -g firebase-tools`
7. Login with your Google account, `firebase login`
8.  Add your project to the sample with `firebase use <project ID>`
  + In Dialogflow console under **Settings** ⚙ > **General** tab > copy **Project ID**.
9. Run `firebase deploy --only functions:dialogflowFulfillment`
10. Back in Dialogflow Console > **Fulfullment** > **Enable** Webhook.
11. Paste the URL from the Firebase Console’s events column into the **URL** field > **Save**.


<sup>A.</sup>In general, **Restore from Zip** will overwrite any existing agent.

<sup>B.</sup>Powered by Cloud Functions for Firebase.

## Samples
| Name                                 | Language                         |
| ------------------------------------ |:---------------------------------|
| [Fulfillment Webhook JSON](https://github.com/dialogflow/fulfillment-webhook-json)| JSON |
| [Dialogflow Console Template](https://github.com/dialogflow/fulfillment-webhook-nodejs)| Node.js
| [Bike Shop-Google Calendar API](https://github.com/dialogflow/fulfillment-bike-shop-nodejs)| Node.js|
| [WWO Weather API](https://github.com/dialogflow/fulfillment-weather-nodejs)| Node.js |
| [Alexa Importer](https://github.com/dialogflow/fulfillment-importer-nodejs) | Node.js |
| [Temperature Trivia](https://github.com/dialogflow/fulfillment-temperature-converter-nodejs) | Node.js |
| [Human-Agent](https://github.com/dialogflow/agent-human-handoff-nodejs) | Node.js |
| [Google Translation API](https://github.com/dialogflow/fulfillment-translate-python) | Python |
| [WWO Weather API](https://github.com/dialogflow/fulfillment-weather-python) | Python |

## References & Issues
+ Questions? Try [StackOverflow](https://stackoverflow.com/questions/tagged/dialogflow) or [Dialogflow Developer Community](https://plus.google.com/communities/103318168784860581977).
+ Find a bug? Report it on [GitHub](https://github.com/dialogflow/fulfillment-webhook-json/issues).
+ Dialogflow [Documentation](https://dialogflow.com/docs/getting-started/basics).
+ For more information on [Initializing Firebase SDK for Cloud Functions](https://firebase.google.com/docs/functions/get-started#set_up_and_initialize_functions_sdk).
+ For more information on [Restore from Zip](https://dialogflow.com/docs/agents#export_and_import)

## Make Contributions
Please read and follow the steps in the CONTRIBUTING.md.

## License
See LICENSE.md.

## Terms
Your use of this sample is subject to, and by using or downloading the sample files you agree to comply with, the [Google APIs Terms of Service](https://developers.google.com/terms/).
