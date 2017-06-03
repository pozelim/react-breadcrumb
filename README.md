# React Breadcrumb Component

[![NPM version][npm-image]][npm-url]
[![npm download][download-image]][download-url]

[npm-image]: http://img.shields.io/npm/v/react-breadcrumb.svg?style=flat-square
[npm-url]: http://npmjs.org/package/react-mf-breadcrumb
[download-url]: https://npmjs.org/package/react-mf-breadcrumb

##Install

`npm install --save react-mf-breadcrumb`

##Examples
```javascript
import Breadcrumb from 'react-breadcrumb';
```
```javascript
<Breadcrumb
  path={'/path/to/section'}
  separatorChar={' - '}
/>
```
Result:
__path__ - __to__ - __section__

**Manual paths**
```javascript
<Breadcrumb
  path={
    [
      {
        path: '/custom/path',
        label: 'path',
      },
      {
        path: '/custom/section',
        label: 'section',
      }
    ]
  }
>  
```


##Props

|Props Name | Type         | Default  | Description              |
|-----------|--------------|:--------:|----------------|
|path       |[string or object]       |          |Path to draw|
|separatorChar|string   |/            |Separator of paths               |
|onClick    |function   |             |Function that takes 2 parameters, event and path clicked|
|className   |String     |            |You can use a custom className|
|classes    |Object |                 |You can customize all classes of component|
