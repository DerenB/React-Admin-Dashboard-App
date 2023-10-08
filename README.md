# React-Admin-Dashboard-App

# Step 0: SyncFusion Components

### Settings Button

```
<div className='fixed right-4 bottom-4' style={{ zIndex: '1000'}}>
  <TooltipComponent content="Settings" position='Top'>
    <button type='button' className='text-3xl p-3 hover:drop-shadow-xl hover:bg-light-gray text-white' style={{ background: 'blue', borderRadius: '50%'}}>
      <FiSettings />
    </button>
  </TooltipComponent>
</div>
```
- The first Div
  - Classes
    - fixed : fixes the location on the screen
    - right-4 : 4 units from the right
    - bottom-4 : 4 units from the bottom
  - Styles
    - zIndex : prioritizes the div so that it is above all other items


# Step 1: Setup Project

- Step 1: Create React App in frontend directory
  - `npx create-react-app frontend`
- Step 2: Delete the `src` folder
  - starts over, removes useless files
  - Create new one
- Step 3: Rebuild `src` items
  - Create Basic React File: `rafce`
  - Create `index.js`
    - React and ReactDOM is imported here
    - `import React from 'react';`
    - `import ReactDOM from 'react-dom';`
  - Create `App.js`
- Step 4: Set up `package.json`
  - Add Dependencies, copy from repo
  - Run: `npm install --legacy-peer-deps`
- Step 5: Add base style sheets to `src`
  - Create `index.css`, add code from Repo
  - Create `App.css`, add code from Repo

### Add Tailwind

- Step 1: Create Tailwind file
  - In main `frontend` directory, create `tailwind.config.js`
  - Add code from repo
- Step 2: Create Craco file
  - In main `frontend` directory, create `craco.config.js`
  - Add code from repo

### Add Directories

- Add all to the `src` directory
- Add `components`
- Add `contexts`
- Add `pages`
- Add `data`
  - downloaded from repo

### Setup index.js

- Add Imports
- Add root render object
```
import React from 'react';
import ReactDOM from 'react-dom';

import './index.css';
import App from './App';

ReactDOM.render(<App />, document.getElementById('root'));
```

### Setup App.js

- Add Imports
```
import React, { useEffect } from 'react';
import { BrowserRouter, Routes, Route } from 'react-router-dom';
import { FiSettings } from 'react-icons/fi';
import { TooltipComponent } from '@syncfusion/ej2-react-popups';

import './App.css';

const App = () => {
  return (
    <h1>App</h1>
  )
}

export default App
```

### Create Components & Page Files

- Add all of the .jsx files
- Create boilerplate code in every file
  - Shortcut: `rafce`