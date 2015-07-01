# \<unity-web-player\>
&lt;unity-web-player> Web Component for Unity3D Web Player. &lt;/unity-web-player>


#####Simple and flexible web component to unity web player games.

[Demo Page](http://cesardeazevedo.github.io/unity-web-player/)

##Get Started

Install using [bower](http://bower.io/)

```sh
$ bower install unity-web-player
````

##Usage

1. Import polyfill

	```html
	<script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
	```

2. Import this custom element

	````html
	<link rel='import' href='bower_components/unity-web-player/unity-web-player.html' />
	```

3. Start using now

	```html
	<unity-web-player source='gameFile.unity3d' name='My Game'></unity-web-player>
	```

###Code Sample

```html
<!DOCTYPE html>
<html>
    <head>
        <title>My Game</title>
        <script src="bower_components/webcomponentsjs/webcomponents.min.js" />
        <link rel="import" href="bower_components/unity-web-player/unity-web-player.html" />
    </head>
    <body>
        <unity-web-player source="mygame.unity3d" width="980" height="465"></unity-web-player>
    </body>
</html>
```

##Options

|Attribute| Type| Default| Description|
|---------|-----|--------|------------|
|source   | String |     | *Required* Path to `.unity3d` file|
|name     | String |     | The name of your game, will show on middle of the screen if `autoplay` is set to false|
|width    | Integer | 980 |Sets the width of the unity web player |
|height   | Integer | 465 | Sets the height of the unity web player|
|autoplay | Boolean |true| If false, will show a play button on middle of screen, otherwise will play game immediately.|
|background| String|| A path to a background image, will show if `autoplay` attribute is set to false |
|text| String|| An aditional text to show when `autoplay` attribute is set to false|
|color| String| black |A color to `name` and `text` attribute|
|playColor|`aqua`, `black`, `darkcyan`, `green`, `pink`, `red`, `white`| `black`| The play button color.|


 
##Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D


##License

[MIT](./LICENSE) Cesar Augusto 


