# Luckysheet
[![Join the chat at https://gitter.im/mengshukeji/Luckysheet](https://badges.gitter.im/mengshukeji/Luckysheet.svg)](https://gitter.im/mengshukeji/Luckysheet?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

English| [简体中文](./README-zh.md)

## Introduction
Luckysheet is an online spreadsheet like excel that is powerful, simple to configure, and completely open source.


## Features
1. Support table settings including freezing columns, merging cells, filtering, sorting, querying, conditional formatting, and annotations
2. Support data analysis functions including pivottables, charts, columns, matrix operations, built-in 385 calculation functions
3. Support one-click screenshots, data copying as json,shared editing, and free data copying and pasting between excel and luckysheet
4. Support mobile viewing
5. Support sparkLine
6. Drop down copy
7. Keyboard shortcuts

![Demo](https://minio.cnbabylon.com/public/luckysheet/LuckysheetDemo.gif)

## Plan
- Improve chart plugin
- Insert picture
- Data validation (checkbox, drop-down list)
- Print
- Cell segmentation style
- Tree menu
- Table function: filter, slice
- Excel import/export
- More...

## Documentation
[Online demo](https://mengshukeji.github.io/LuckysheetDemo/)

[Online documentation](https://mengshukeji.github.io/LuckysheetDocs/)

## Requirements
[Node.js](https://nodejs.org/en/) Version >= 6 

## Installation
```
npm install
npm install gulp -g
```

## Development
Development
```
npm run dev
```
Package
```
npm run build
```
Read

The core code of Luckysheet is luckysheet-core.js and luckysheet-function.js, developers only need to look at these two files to see the source code, and then we will discuss the modularization scheme and improve this library.

## Usage

#### First step
Copy all files in the `dist` folder after `npm run build` to the project directory

#### Second step
Introduce dependencies
```
<link rel='stylesheet' href='./plugins/css/pluginsCss.css' />
<link rel='stylesheet' href='./plugins/plugins.css' />
<link rel='stylesheet' href='./css/luckysheet.css' />
<script src="./plugins/js/plugin.js"></script>
<script src="./luckysheet.umd.js"></script>
```
#### Third step
Specify a table container
```
<div id="luckysheet" style="margin:0px;padding:0px;position:absolute;width:100%;height:100%;left: 0px;top: 0px;"></div>
```
#### Fourth step
Create a table
```
<script>
    $(function () {
        //Configuration item
        var options = {
            container: 'luckysheet' //luckysheet is the container id
        }
        luckysheet.create(options)
    })
</script>
```

## Contact
mengshu@office2.cn

## communication

- [Gitter](https://gitter.im/mengshukeji/Luckysheet)

## Authors and acknowledgment
- [@wpxp123456](https://github.com/wpxp123456)
- [@Dushusir](https://github.com/Dushusir)

## License
[MIT](http://opensource.org/licenses/MIT)

Copyright (c) 2020-present, mengshukeji
