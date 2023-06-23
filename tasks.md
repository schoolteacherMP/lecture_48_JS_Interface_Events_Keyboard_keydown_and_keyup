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
### СЕКРЕТНАЯ последовательность клавиш A, B, C    
Создайте HTML-страницу без текстовых полей ввода.   
`<style>`  
      `#imgTask9{`  
        `display: none;`  
        `position: absolute;`  
        `top:0;`  
        `width: 100vw;`  
        `height: 100vh;`  
        `background-color: black;`  
      `}`  
    `</style>`  
    `<img src="7B97.gif" alt="Задача9" id="imgTask9">`  
Напишите JavaScript-код, который будет отслеживать событие "keydown" и проверять, была ли нажата последовательность клавиш "A", "B", "C" (в таком порядке).   
Если это так, выведите в alert: "Нажата СЕКРЕТНАЯ последовательность клавиш A, B, C".  
Затем следует задать вопрос с помощью confirm: Вы осознаете последствия?  
И если нажата клавиша OK - показать на весь экран картинку (произвольную), должна перекрыть весь экран.  
По истечению 5 секунд она должна исчесзнуть.  
PS: на помощь придет [setTimeout](https://developer.mozilla.org/ru/docs/Web/API/setTimeout).   
Скачать гифку можно [тут](https://gifer.com/ru/7B97)  

https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/c7c8ca07-a823-496b-9158-e26ab5863e71   

**Шаги выполнения могут быть такими:**  
1. Создается пустой массив **pressedKeys**, который будет использоваться для сохранения нажатых клавиш.  

2. Добавляется обработчик события "**keydown**" для документа.     
При каждом нажатии клавиши вызывается функция-обработчик события, которая добавляет нажатую клавишу в массив pressedKeys и затем вызывает функцию `checkSequence()` для проверки последовательности клавиш.  
3. Функция `checkSequence()` определяет заданную последовательность клавиш в массиве `sequence (["a", "b", "c"])`.  

4. Проверяется, достаточно ли клавиш уже нажато в массиве pressedKeys, чтобы сравнить с заданной последовательностью. Если длина массива pressedKeys больше или равна длине sequence, то выполняется дальнейшая проверка.  

5. Создается подмассив `lastKeys`, содержащий последние три элемента массива pressedKeys. Мы используем `pressedKeys.slice(-3)` для получения последних трех элементов, так как в заданной последовательности есть три клавиши.  

6. Сравнивается соединенная строка `lastKeys.join("")` с соединенной строкой заданной последовательности `sequence.join("")`. Если они совпадают, выводится предупреждающее сообщение _"Нажата СЕКРЕТНАЯ последовательность клавиш A, B, C"_.  

7. После вывода предупреждающего сообщения, вызывается функция `confirm()`, которая отображает диалоговое окно с вопросом _"Вы осознаете последствия?"_.
   Результат ответа пользователя сохраняется в переменную `confirmAnswer`.  

8.Если `confirmAnswer` равно `true` (пользователь нажал кнопку "ОК"), выполняются следующие действия:  

- Устанавливается свойство display элемента с идентификатором imgTask9 в значении 'block', что приводит к отображению соответствующей картинки.  
- Затем, с помощью setTimeout(), запускается функция, которая устанавливает свойство display элемента imgTask9 в 'none' через 5 секунд (5000 миллисекунд).  
- Таким образом, картинка будет отображена в течение 5 секунд, а затем исчезнет.  



## Задача 8.   
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


## Задача 9.   
### Задача на предотвращение действий по умолчанию при нажатии определенных клавиш:  
Создайте HTML-страницу с текстовым полем ввода.   
Напишите JavaScript-код, который будет отслеживать событие "keydown" и проверять, является ли нажатая клавиша клавишей "Space".   
Если это так, предотвратите стандартное действие при нажатии клавиши "Space" и выведите в консоль: "Нажата клавиша Space".  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/8543fee7-8de8-467d-b33f-297d7deac4fc)  
![image](https://github.com/schoolteacherMP/lecture_48_JS_Interface_Events_Keyboard_keydown_and_keyup/assets/113675674/6cb52890-0b78-4909-a7d6-4d9402e74518)  





    
