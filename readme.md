# Iniciando um projeto REACTjs TAILWINDcss

### 1.
``` NPM
npm create react-app exemplename
```

### 2.
``` CMD
cd exemplename
```

### 3.
``` GIT
git init
```

### 4.
``` GIT
git config --global user.email "you@example.com"
```

### 5.
``` GIT
git config --global user.name "Your Name"
```

### 6.
``` GIT
git branch -M main 
```

### 7.
``` GIT
git remote add origin https://github.com/exemple-user/exemple-repo.git
```

### 8.
``` GIT
git push --set-upstream origin main
```

### 9.
> Dentro da pasta src exclua os arquivos App.css, App.test.js, logo.svg, reportWebVitals.js, setupTests.js

### 10.
> O arquivo App.js deve ficar da seguinte forma:
``` JS
function App() {
  return (
    <h1>Hello World</h1> 
  );
}

export default App;
```

### 11.
> O arquivo index.js deve ficar da seguinte forma:
``` JS
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import App from './App';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<App />);
```

### 12.
``` NPM
npm install -D tailwindcss
```

### 13.
``` NPM
npx tailwindcss init
```

### 14.
> O arquivo tailwind.config.js deve ficar da seguinte forma:
``` JS
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### 15.
> Adicione os seguintes códigos no arquivo index.css:
``` JS
@tailwind base;
@tailwind components;
@tailwind utilities;
}
```