#### For Intel XDK
Use `onesignal-cordova-plugin` instead if you **NOT** using Intel XDK.

#### Description
This adds required Android dependencies needed by OneSignal. Use this plugin along with `onesignal-cordova-plugin-pgb-compat` when building with Intel XDK.

#### Why this is required
This was created as the main branch of the OneSignal Cordova plugin `onesignal-cordova-plugin` uses a gradle script which Intel XDK does not allow. Using older .jar Cordova projects for Google Play services and Android Support library were recommended in the past but they are not compatable with newer plugins that use .aar sytle gradle compile entires. This is due to duplicate Java classes being defined which creates Cordova build errors durning the dex step.