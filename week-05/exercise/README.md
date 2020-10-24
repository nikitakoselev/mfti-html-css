#Task definition
Необходимо:

Анимировать облака. Облака повернуть в разные стороны.
Они разных размеров и движутся с разной скоростью. 
Те, что ближе к зрителю, — больше и движутся быстрее. 
Те, что дальше, — меньше и медленнее.

Анимировать солнце. 
Оно движется по кругу и вращается вокруг своей оси.

Пароход. 
Движется равномерно. 
Элементы, которые представляют собой дым, 
увеличиваются и меняют прозрачность (см. видео).

Фон меняется синхронно с восходом и заходом солнца. 
У неба есть 3 состояния: день, вечер, ночь. 
В коде есть все 3 состояния, 
нужно реализовать плавный переход между ними и зациклить его.

#*******************
#Notes from lectures

#The solution is mostly based on the "transform" CSS
transform: transformation-type-here
*translateX
*scale (X/Y/+ -)
*rotate (turn/degrees)
*skew 
*transform-origin #changes the rotation point
*rotate

#advanced
backface-visibility
rotate3d

#transformations matrix

#transitions
transition-property
transition-duration
transition-timing-function

#css animations
@keyframes 
from-to
0% 5% ... 100%
animation-timing-function
animation-duration
animation-delay
animation-iteration-count: d, infinite
animtion-direction: alternate/
animation-fill-mode: forwards

#alternative to long list of animations:
animation: scale 2s ease-in-out 3 alternate 5s forwards
animation: scale 2s ease-in, move 2s ease-out
div {
  animation: anim 5s;
}

#1 sec pause
@keyframes anim {
  0% {
    color: red;
  }
  40%, 60% {
    color: blue;
  }
  100% {
    color: green;
  }
}

#controlling the state
animation-play-state: paused;
