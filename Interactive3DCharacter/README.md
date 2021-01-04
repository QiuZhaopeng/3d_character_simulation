# 3d_character_simulation

## Execution

Run the following cmd:
    npm install
	npm start
	
	
## Control singal sending 


One can write his own program to send angle via websockt. Angle data (two int16) to be sent should be written into msg_send_posture[8:9] and msg_send_posture[10:11]. Example code:
	var wsUrl = "ws://localhost:9999";

	websocket = new WebSocket(wsUrl);
	var msg_send_posture  =  new Uint8Array([0xAA,  0x01,0x53,  0x01,  0x04,0x00,0x00,0x00,   0x01,0x00, 0x00,0x00,  0x00,0x00,   0x7F];

	websocket.send(msg_send_posture);
  




## Original Project: Interactive 3D Character with Three.js

Demo for the tutorial on how to add an interactive 3D character to a website.

![3D Character](https://tympanus.net/codrops/wp-content/uploads/2019/10/Interactive3DCharacter_feat.jpg)

[Article on Codrops](https://tympanus.net/codrops/?p=43796)

[Demo](http://tympanus.net/Tutorials/Interactive3DCharacter/)

### Credits

- [three.js](https://threejs.org/)

### License
This resource can be used freely if integrated or build upon in personal or commercial projects such as websites, web apps and web templates intended for sale. It is not allowed to take the resource "as-is" and sell it, redistribute, re-publish it, or sell "pluginized" versions of it. Free plugins built using this resource should have a visible mention and link to the original work. Always consider the licenses of all included libraries, scripts and images used.

### Misc

Follow Kyle: [Twitter](https://twitter.com/KyleWetton), [Codepen](https://codepen.io/kylewetton/), [LinkedIn](https://www.linkedin.com/in/kylewetton/)

Follow Codrops: [Twitter](http://www.twitter.com/codrops), [Facebook](http://www.facebook.com/codrops), [GitHub](https://github.com/codrops), [Instagram](https://www.instagram.com/codropsss/)


[© Codrops 2019](http://www.codrops.com)





