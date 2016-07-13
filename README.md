# elis
A node module for utility in Electron.

##Introduction
An 'is' utility for Electron.  
`elis` provides a set of isomorphic 'is' APIs, that you can use it both in main and renderer process.  

##install
    npm install elis --save
##API
- **is.renderer()**  
Returns `true` if you are calling the function from the renderer process.

- **is.main()**  
Returns `true` if you are calling the function from the main process.

- **is.osx()**  
Returns `true` if your app is running under Mac OS.

- **is.windows()**  
Returns `true` if your app is running under Windows OS.

- **is.linux()**  
Returns `true` if your app is running under Linux OS.

- **is.x86()**  
Returns `true` if you the architecture of the processor is `ia32`.

- **is.x64()**  
Returns `true` if you the architecture of the processor is `x64`.

- **is.isWin7plusOS()**  
Returns `true` if you OS is more than `windows 7`.

##usage
    var is = require('elis');
    console.log(is.ismain());//true or false