## Задача 1.   
### "shift" и "w"  
Когда пользователь нажимает клавиши `"shift"` и `"w"` одновременно, вывести с помощью `alert()` сообщение: `'Ответ на главный вопрос жизни, вселенной и вообще - 42'.`    
Нужно добавить обработчик события нажатия клавиш на документ. Когда пользователь нажимает клавиши `"shift"` и `"w"` одновременно, обработчик события проверяет, соответствует ли код нажатой клавиши `"KeyQ"` и `"KeyW"`. Если это так, то вызывается функция `alert()`, которая выводит сообщение.  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/37908ea4-8694-4511-9f8d-179c864cec68)  


## Задача 2.   
### цвет фона  
Напишите код, который добавляет обработчики событий `keydown` и `keyup` на документ.   
Когда пользователь нажимает клавиши `"Shift"` и `"q"` одновременно, обработчик события `keydown` проверяет, соответствует ли код нажатой клавиши `"KeyQ"` и была ли нажата клавиша `"Shift"`.  
Если это так, то задается фоновый цвет элемента `myDiv` в красном цвете.  
Когда пользователь отпускает любую из этих клавиш, обработчик события `keyup` сбрасывает цвет обратно на прежний.  
PS: `event.shiftKey` - для `"Shift"`  

`HTML`  
`<div id="myDiv"></div>`  
`CSS`  
`#myDiv {`  
  `width: 100%;`  
  `height: 200px;`  
  `background-color: green;`  
`}`  


## Задача 3.   
###   отображения текста  
Создание простого приложения для отображения текста при нажатии на клавишу.  
`word-wrap: break-word;` - чтобы текст, который не влазит в div, переносился на новую строку.  
Т.е. при нажатии на клавишу, должно отображаться в `<div id="output">` значение клавиши которое вы нажали.  
PS: `textContent`, `event.key`   
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/56e9f6c9-dff7-4132-a753-7e2abb23ff3d)  

`HTML`  
`<div id="output"></div>`  
`CSS`  
`#output{`  
  `width: 300px;`  
  `height: 200px;`  
  `background-color:blueviolet;`  
  `color: azure;`  
  `word-wrap: break-word;`  
`}`  


## Задача 4.   
### Счетчик нажатий клавиш  
Напишите код, который позволит подсчитать колличество нажатых клавиш и обновляет отображение счетчика в элементе с **id="count"**.  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/ee919dd4-20aa-40bb-b007-1cca942e3b5b)  

`HTML`  
`<div class="wrapper_count">Нажато клавиш: <span id="count">0</span></div>`  
`CSS`  
`.wrapper_count{`  
  `width: 300px;`  
  `height: 50px;`  
  `background-color:blue;`  
  `color: azure;`    
`}`  


## Задача 5.   
### Отображение символа, нажатого пользователем, на экране.  
Напишите код, который будет отображать в параграфе **id="result"**  символ, который нажал пользователь, как только пользователь отпустил клавишу символ должен исчезать из параграфа **id="result"** .   
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/106743a5-9df0-4aa5-8243-2bdea279acc5)  

`HTML`  
 `<div class="wrapper_result">`  
   `<h2>Введите символ:</h2>`  
   `<p id="result"></p>`  
 `</div>`  
   `CSS`  
`.wrapper_result{`  
  `width: 300px;`  
  `height: 100px;`  
  `background-color:chocolate;`  
`}`  
`#result{`  
  `font-size: 46px;`  
  `margin: 0 auto;`  
  `width: 100px;`  
`}`  
   

## Задача 6.   
### Увеличение размера шрифта при зажатой клавише Shift.  
Напишите код, который будет увеличивать размер шрифта в `h2` на `'2em'`, когда пользователь нажмет клавишу `Shift` и возвращать в первоначальное состояние, когда пользователь отпустит клавишу `Shift`.   
PS: `style.fontSize = '2em';`  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/cf73e86e-10d7-4501-a979-40bd2fcffcd1)  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/7652e41a-139c-42dc-9534-615155742b98)  


`HTML` 
`<h2 id="test_shift">Нажмите на клавишу Shift</h2>`   

## Задача 7.   
### Увеличение размера шрифта при зажатой клавише Shift + Click.    
Есть две кнопки: button1 и button2, а также три блока текста, которые будут изменять свой размер шрифта при клике на кнопки.  
Кнопка button1 увеличивает размер шрифта на 2 пикселя при клике, если при этом зажата клавиша Shift.   
Кнопка button2 уменьшает размер шрифта на 2 пикселя при клике, если при этом зажата клавиша Shift.    
PS: Размер шрифта начинается с 16 пикселей и изменяется для всех div-элементов на странице.   
Следует воспользоваться в обработчике методом передора forEach. А для этого у вас должна быть коллекция элементов ;)  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/57d9ca4e-acda-4014-8d6c-25d9ad03708d)  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/4fb7d488-6bf3-4f81-82b1-b7c8f245ed6b)  



`<button id="button1">Нажми, удерживая 'Shift', что бы +</button>`  
    `<button id="button2">Нажми, удерживая 'Shift', что бы -</button>`  
    `<div>`  
      `Можешь говорить что угодно, но пирожное я заберу.`  
      `<div>`  
        `Нельзя выиграть, если ты только защищаешься. Чтобы выиграть, нужно идти в атаку.`  
        `<div>`  
          `— Интересно, сколько там было? Наверное миллионов десять?`  
          `— А сколько это в яблоках?`  
        `</div>`  
      `</div>`  
    `</div>`  
    
`button {`  
  `padding: 10px 20px;`  
  `font-size: 16px;`  
  `border-radius: 5px;`  
  `margin-right: 10px;`  
`}`  

`#button1 {`  
  `background-color: green;`  
  `color: white;`  
`}`  

`#button2 {`  
  `background-color: red;`  
  `color: white;`  
`}`  

    
