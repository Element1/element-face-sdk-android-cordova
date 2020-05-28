![element](../images/element.png "element")
# Element Face Cordova Plugin

## Install Element Face SDK and EAK
- Please contact Element to access the files.
- Replace the placeholder files in the [folder](./src/android).

## Integrate with existing cordova app
Please see the [example](../element-cordova-face-sdk-example/readme_images/README.md).

## Launcher [Functions](./www/element.js)
Each method below has a success and failure callback that will be called at the end of the process. All inputs are Strings.

### create
Adds a new untrained user to the internal data store. It is up to the client to validate each field based on their business requirements.
Requires **userId**, **firstname**, **lastname**

### train
Start training a user that was previously created using the **create** method above.
Requires **userId**

### authentication
Initiate a face authentication for the given userId.
Requires **userId**

### list
Polls the Element data store to get a full list of users as a JSON array.

## Customization
New SDK support some customization, although still need to be done in android way. You can customize your `plugin.xml` file to add `string` or resources that available in this [docs](https://github.com/Element1/element-face-sdk-android/blob/master/docs/element-face-ui.md).