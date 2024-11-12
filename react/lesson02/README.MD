# Створюємо компоненти
## Створимо компонент info
1. В папці `src` створимо папку `components`
2. В папці `components` створимо файл `info.js`
```js
import React from "react";

class Info extends React.Component{
    render(){
        return(
            <div>
                <h2>Інформаційний заголовок</h2>
                <p>Інформація</p>
            </div>
        );
    }
}
```
export default Info;

в файлі `app.js` іпортуємо файл `info.js`:

В заголовку пишемо:
```js
import Info from "./components/info"
```
в **render** ставимл

`<Info />` в місці де необхідно вивести результат роботи відповідного компоненту.
