# Season Share SDK 
This plugin enables teams to include Season Share capabilities within their own mobile applications. 
You can learn more about Season Share at https://seasonshare.com

🛠 In order for us to provide optimal support, we would kindly ask you to submit any issues to sdk@seasonshare.com

When submitting an issue please specify your Season Share App ID, SDK version, team name, production steps, logs, dependency declaration files, code snippets and any additional relevant information.

## React Native 

### 📲 Adding the SDK to your project 

1. Request access to SS Plugin NPM Package via GitHub. 
2. Install the plugin from your mobile application root directory
    `$ npm install --save seasonshareapp/ss-sdk`

Then run the following:
#### iOS

`$ cd ios && pod install`
`$ react-native run-ios`

The SDK utilizes React-Native autolinking. If you are integrating with a version of RN that does not support autolinking, you will need to manually link the SeasonShare binary in your XCode project's build phases. 

#### Android
`$ react-native run-android`

You may need to specify 

## 🚀 Invoking the SDK

```
import { Text } from 'react-native';
import SeasonShare from 'ss-sdk';
 
const MySeasonShareComponent = () => {
  return (
    <SeasonShare
     // Replace any of the following <#VARIABLE#>s according to your setup,
     
      ssApiKey='<# Your Season Share API Key #>'
      ssAppId='<# Your Season Share App Id #>'
      primaryColor='<# Hex color code - primary #>'
      secondaryColor='<# Hex color code - secondary #>'
      onSuccess={data => console.log('success: ', data)}
      onExit={data => console.log('exit: ', data)}
 
      // Optional props
      loggedInUsserEmailAddress='<# User Email #>'
      loggedInUserFullName='<# User Full Name #>'
    >
    </SeasonShare>
  );
};
```
## Demo
![alt text](https://media.giphy.com/media/SSKp1ae2kNn4ipxSdw/giphy.gif "Logo Title Text 1")














