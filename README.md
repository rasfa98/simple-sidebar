# Simple Sidebar

A simple sidebar to use in your React project!

## Features

- Responsive
- Animated
- Overlay with close sidebar feature
- Easy to use
- Customize overlay color and sidebar background

## Installation

`npm install simple sidebar`

## How to use

```js
import React, { useState } from "react";

import Sidebar from "simple-sidebar";

const App = () => {
  const [isOpen, setIsOpen] = useState(false);

  return (
    <Sidebar
      options={{ overlay: "rgba(0, 0, 0, 0.8)", background: "darkseagreen" }}
      isOpen={isOpen}
      onClose={() => setIsOpen(false)}
      content={<div>This is the sidebar content!</div>}
    >
      <div className="App">
        <button onClick={() => setIsOpen(true)}>Open sidebar</button>
      </div>
    </Sidebar>
  );
};

export default App;
```
