# JS_Week11
Hometask for Week 11 Javascript, DOM, functions, events

### Вопросы 💎

1. Сколько детей (дочерних DOM-узлов) у элемента `<ul>` в примере ниже:
    2 (<li>Привет</li>
        <li>Мир</li>)
        
    ```jsx
    <ul>
        <li>Привет</li>
        <li>Мир</li>
    </ul>
    ```
    
2. Есть такой элемент: `<input id= "input" value = "Привет">`. Какой вызов поменяет значение в нём?
3. Сколько потомков будет у `<div>` после кода ниже?
    
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
- Когда у elem единственный потомок
- Когда у elem нет потомков
- Нет такого варианта ответа
5. Какое свойство задает класс элемента?
6. Для чего используется запись: `setAttribute(name, value)`?
7. Назовите метод добавления текста к документу.
8. Как получить HTML-содержимое DOM-элемента elem?
9. Что такое объект события и какие у него могут быть свойства?
10. Что такое BOM и DOM?
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
    2. Все элементы `label` **внутри** этой таблицы (их три)
    3. Форму `form` с именем `name="search-person"`
12. Как сделать переход на другую страницу при клике на кнопку (без `<a href=...>`, только средствами JavaScript)?
