# Temperature Trivia

## Setup
Select **only one** of the options below.

### Option 1: Add to Dialogflow (Recommended)
To create this agent from our template:

<a href="https://console.dialogflow.com/api-client/oneclick?templateUrl=https://oneclickgithub.appspot.com/dialogflow/fulfillment-temperature-converter-nodejs&agentName=TemperatureSample" target="blank">
  <img src="https://dialogflow.com/images/deploy.png">
</a>


### Option 2: Firebase CLI
1. Create a [Dialogflow Agent](https://console.dialogflow.com/).
2. `git clone https://github.com/dialogflow/fulfillment-temperature-converter-nodejs.git`
3. Go to **Settings** ⚙ > **Export and Import** > **Restore from zip** using the `dialogflow-agent.zip` in this directory.
4. `cd` to the `functions` directory
5. Run `npm install`.
6. Install the Firebase CLI by running `npm install -g firebase-tools`
7. Login with your Google account, `firebase login`
8.  Add your project to the sample with `firebase use <project ID>`
      + In Dialogflow console under **Settings** ⚙ > **General** tab > copy **Project ID**.
9. Run `firebase deploy --only functions:dialogflowFulfillment`
10. Back in Dialogflow Console > **Fulfullment** > **Enable** Webhook.
      + Paste the URL from the Firebase Console’s Trigger column under the **Functions > Dashboard** tab into the **URL** field > **Save**.


## Related Samples
| Name       | Language           |
| ------------- |:-------------:|
| [Fulfillment & Regex Validation](https://github.com/dialogflow/fulfillment-regex-nodejs)      | Node.js |
| [Weather: Fulfillment & WWO API](https://github.com/dialogflow/fulfillment-weather-nodejs)     | Node.js      |  
| [Bike Shop: Fulfillment & Google Calendar API](https://github.com/dialogflow/fulfillment-bike-shop-nodejs)| Node.js |
| [Temperature Trivia: Fulfillment & Actions on Google](https://github.com/dialogflow/fulfillment-temperature-converter-nodejs) | Node.js |
| [Fulfillment & Actions on Google](https://github.com/dialogflow/fulfillment-actions-library-nodejs) | Node.js |
| [Fulfillment & Firestore Database](https://github.com/dialogflow/fulfillment-firestore-nodejs) | Node.js |
| [Multi-language/locale](https://github.com/dialogflow/fulfillment-multi-locale-nodejs) | Node.js |
| [Basic Slot Filling](https://github.com/dialogflow/fulfillment-slot-filling-nodejs) | Node.js |
| [Alexa Importer](https://github.com/dialogflow/fulfillment-importer-nodejs) | Node.js |

For Fulfillment Webhook [JSON Requests & Responses](https://github.com/dialogflow/fulfillment-webhook-json).

## References & Issues
+ Questions? Try [StackOverflow](https://stackoverflow.com/questions/tagged/dialogflow) or [Dialogflow Developer Community](https://plus.google.com/communities/103318168784860581977).
+ Find a bug? Report it on [GitHub](https://github.com/dialogflow/fulfillment-webhook-json/issues).
+ Dialogflow [Documentation](https://dialogflow.com/docs/getting-started/basics).
+ For more information on [Initializing Firebase SDK for Cloud Functions](https://firebase.google.com/docs/functions/get-started#set_up_and_initialize_functions_sdk).
+ For more information on [Restore from Zip](https://dialogflow.com/docs/agents#export_and_import).

## Make Contributions
Please read and follow the steps in the CONTRIBUTING.md.

## License
See LICENSE.md.

## Terms
Your use of this sample is subject to, and by using or downloading the sample files you agree to comply with, the [Google APIs Terms of Service](https://developers.google.com/terms/).
