# JS_Week11
Hometask for Week 11 Javascript, DOM, functions, events

### Вопросы 💎
1. Сколько детей (дочерних DOM-узлов) у элемента `<ul>` в примере ниже:
*2 li*
    
    ```jsx
    <ul>
        <li>Привет</li>
        <li>Мир</li>
    </ul>
    ```
    
2. Есть такой элемент: `<input id= "input" value = "Привет">`. Какой вызов поменяет значение в нём? 
`*document.getElementById('input').value = 'changed Value';*`

3. Сколько потомков будет у `<div>` после кода ниже?
*3*

    
    ```jsx
    <div id="div"></div>
    <p id="p">Привет</p>
    
    <script>
      div.append(p);
      div.append(p);
    </script>
    ```
    
4. В каких случаях для элемента elem не верно `elem.firstChild == elem.lastChild`?
- Когда у elem два или более потомков
- Когда у elem нет потомков
- Нет такого варианта ответа

5. Какое свойство задает класс элемента?
***.classList.add('**');*

6. Для чего используется запись: `setAttribute(name, value)`?
*Для задания значения атрибута (name - имя атрибута, value - значение, которое хотим задать)*

7. Назовите метод добавления текста к документу.
*Свойство textContent* 

8. Как получить HTML-содержимое DOM-элемента elem?
*elem.innerHTML;*

9. Что такое объект события и какие у него могут быть свойства?

Объект события содержит в себе детали произошедшего в браузере. 
Свойства зависят от типа события, но, например, у события мыши есть следующие свойства
- click
- contextmenu
- mouseover/mouseout
- mousedown/mouseup
- mousemove*

10. Что такое BOM и DOM?

BOM - Browser Object Model - дополнительные объекты, предоставляемые браузером (окружением), чтобы работать со всем, кроме документа.
DOM - Document Object Model -  HTML-разметка: блоки, из которых состоит документ.

11. Есть вот такая страница:
    
    ```html
    <!DOCTYPE HTML>
    <html>
    
    <body>
    	<form name="search">
    		<label>Поиск:
    			<input type="text" name="search"> </label>
    		<input type="submit" value="Search!"> </form>
    	<hr>
    	<form name="search-person">Поиск по посетителям:
    		<table id="age-table">
    			<tr>
    				<td>Возраст:</td>
    				<td id="age-list">
    					<label>
    						<input type="radio" name="age" value="young">до 18</label>
    					<label>
    						<input type="radio" name="age" value="mature">18-50</label>
    					<label>
    						<input type="radio" name="age" value="senior">старше 50</label>
    				</td>
    			</tr>
    			<tr>
    				<td>Дополнительно:</td>
    				<td>
    					<input type="text" name="info">
    					<input type="text" name="info">
    					<input type="text" name="info"> </td>
    			</tr>
    		</table>
    		<input type="button" value="Search!"> </form>
    </body>
    
    </html>
    ```
    
    Как найти в ней:
    
    1. Таблицу с `id="age-table"`
    *document.getElementById(’age-table’);*
    
    2. Все элементы `label` **внутри** этой таблицы (их три)
    *document.querySelectorAll(’.label’);*
    
    3. Форму `form` с именем `name="search-person"`
    *document.getElementByTagName(’search-person’);*
    
12. Как сделать переход на другую страницу при клике на кнопку (без `<a href=...>`, только средствами JavaScript)?

*let button = document.getElementById("elem");
button.onclick = function() { document.location=’ссылка’;};*
