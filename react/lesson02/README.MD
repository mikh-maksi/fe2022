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

export default Info;
```

в файлі `app.js` іпортуємо файл `info.js`:

В заголовку пишемо:
```js
import Info from "./components/info"
```
в **render** ставимо

`<Info />` в місці де необхідно вивести результат роботи відповідного компоненту.

Основний файл у нас буде виглядати наступним чином:
```js
import man from './man.png';
import './style.css';
import Info from "./components/info"

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <img src={man} />
        <p>
         Hello! My name in <b>Man</b>. Glad to see you.
        </p>You would take diffirent images here: &nbsp; 
        <a
          className="App-link"
          href="https://www.iconfinder.com/"
          target="_blank"
          rel="noopener noreferrer"
        > 
          Iconfinder.
        </a>
      </header>
      <Info />

    </div>
  );
}

export default App;

```
