# Pavel Grinkevich

## My Contacts

 - **Email**: pavel.grinkevich@gmail.com
 - **Github**: github.io/elquespera
 - **Phone**: +420 608831542

## My Goals

I'm a scientist/amateur developer who aims to become a professional **front-end developer**. I've been coding on and off since I was little, then switched to my Biophysics degree. Now I want to try my hand at coding again.

## My Skills

 - HTML/CSS
 - JavaScript

## My Code

```
//plot random walk trajectories in random colors from 2d array
function markovPlot(trajectories, canvas) {
	scaleX = canvas.width / trajectories[0].length;
	scaleY = scaleX;
	startY = Math.round(canvas.height / scaleY / 2);
	startX = 0;
	context = canvas.getContext("2d");
	context.clearRect(0, 0, canvas.width, canvas.height);
	for (i = 0; i < trajectories.length; i++) {
		x = startX; y = startY;
		context.beginPath();
		context.strokeStyle = '#'+Math.floor(Math.random()*16777215).toString(16);
		context.moveTo(x * scaleX, y * scaleY);
		for (j = 1; j < trajectories[i].length; j++) {
			x += scaleX;
			y = (startY + trajectories[i][j]) * scaleY;
			context.lineTo(x, y);
			context.stroke();
		}
	}
}
```

## My Languages
 - English, **C1**, fluent
 - Russian, **native**
 - Czech, **B1**
