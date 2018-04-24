# SyncProxy step-by-step quick start guide for Ionic
This is a quick start tutorial to how to setup an Ionic hybrid mobile application embedding its own database together with **SyncProxy** client. Used with online **SyncProxy** server (www.syncproxy.com), this is the quickest way to create applications that will synchronize bidirectionally, reactively in realtime with your backend database (MySQL, SQL Server, MongoDB...), and also work perfectly when offline. *Only with one line of code.*

## Architecture
The **SyncProxy** client targets hybrid mobile applications (Ionic, Phonegap, Cordova, Xamarin...) with an embedded database (IndexedDB, SQLite, WebSQL...) that provides offline capabilities. By adding the **SyncProxy** client to your main .html file **with one single line of code**, you will turn your offline app into a powerfull online application with bidirectionnal reactive (realtime) sync that will work perfectly with or without connection. You will not need develop any specialized webservices, since the **SyncProxy** server enables to define sync profiles directly online on www.syncproxy.com which acts as a gateway between your app and your backend database.

## How to setup an existing Ionic application
To get your existing Ionic application ready with the **SyncProxy** client:
 1. Download the [**SyncProxy** client](https://github.com/hmellanger/syncproxy-client) and copy it into the /src/assets/ folder of your Ionic project.
 2. Add the followin line in the &lt;body&gt; section of your *index.html* file located in the */src/* folder of your Ionic project (replace *proxyId* attribute with the id allocated during the online creation of the proxy):
````html
<script src="sync-client/sync-client.js" serverUrl="localhost" proxyID="kMrtc82xffw2ZrPf6"  connectorType="IndexedDB" dbName="your-client-db-name"></script>
````

## How to create a new application

````javascript
````

## Link
To access SyncProxy administration to setup your sync proxy and connect to your database, go to www.syncproxy.com
