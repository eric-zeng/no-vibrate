This is the hello world app created by the ```cordova create``` command, 
with the cordova-plugin-local-notifications plugin installed. On deviceready,
it fires a single notification, with vibrate and sound set to false, and
priority set to -2. 

```
cordova.plugins.notification.local.schedule({
    id: 0,
    title: 'Testing notification',
    text: 'Vibrate set to false, sound set to false, priority set to min',
    vibrate: false,
    sound: false,
    priority: -2
});

```

The relevant code is in:
https://github.com/eric-zeng/no-vibrate/blob/master/www/js/index.js


How to reproduce:
1. Clone the repository
2. ```cordova run android```
3. Open the app
4. Notification should fire on open

