
## HI evryone!!!! 
# This's my CV
|________| |![me](/photo/me.jpg))| |_________|
### _ ABOUT ME _

> i`m 18 years old, i study in the minsk trade college. Last ear i finished my firs course it was Js-Frond-end stage0. i alawys want to try coding. So now im a beginir in js and IT.

*for exsemple my code*

```
 function gameLoop () {

    requestAnimationFrame(gameLoop);
    if (++settigs.step < settigs.maxStep) {
        return;
    }
    settigs.step = 0
    context.clearRect(0, 0, canvas.width, canvas.height)
    drawSnake()
    drawBary()
}

function drawSnake () {
    snake.x = snake.x + snake.speedX
    snake.y = snake.y + snake.speedY
    snake.taill.unshift({x: snake.x, y: snake.y})
    spaunBackWall()
    if (snake.taill.length > snake.maxataill) {
       snake.taill.pop()
    }
    snake.taill.forEach((value, index) => {
        
        
        if (index === 0) {
            context.fillStyle = '#eb5757'
        }
        if (index > 0) {
            context.fillStyle = '#72de0d'
        }
        context.fillRect(value.x, value.y, settigs.sizeCell, settigs.sizeCell)
        
        if (value.x === barry.x && value.y === barry.y) {
            snake.maxataill++
            plusScore()
            setRandomBarry()
        }
        for (let i = index + 1; i < snake.taill.length; i++) {
            if (value.x === snake.taill[i].x && value.y === snake.taill[i].y) {
                refrechGame()
            }
        }
    })
    
}
```
***My progect***
[my progect](https://rolling-scopes-school.github.io/timkahi-JSFEPRESCHOOL/Portfolio/ "progect from stage0")

