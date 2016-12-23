# JS Notify


##Requirements

* Enabled JavaScript in browser
* jQuery installed

##Installation

Run:

```bower install jsnotify```

Add the following between your projects ```head``` tags:

```html
<!-- JsNotify Style -->
<link rel="stylesheet" href="bower_components/jsnotify/src/style.css">
```

And the following just before your projects closing ```body``` tag:

```html
<!-- JsNotify Script -->
<script src="bower_components/jsnotify/src/notify.js"></script>
```

##Usage

```javascript

var options = {
	'title': 'Oi!',
	'message': 'Whatever you did, it worked!',
	'icon': 'check',
	'style': 'success'
};

var n = new notify(options);

n.show();
```

##Options

| Option        | Required | Description                                                                                          |
|---------------|----------|------------------------------------------------------------------------------------------------------|
| ```title```   | No       | The title of the notification, this will appear at the top of the notification.                      |
| ```message``` | Yes      | This is the body of the notification.                                                                |
| ```icon```    | No       | The icon to be used within the notification, this is displayed at the left side of the notification. |
| ```style```   | No       | Style of the notification. Can be ```default```, ```success``` or ```error```.                       |