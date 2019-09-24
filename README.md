# g2plot : a charting library based on the Grammar of Graphics


[![版本](https://badgen.net/npm/v/@antv/g2plot)](https://www.npmjs.com/@antv/g2plot)
[![NPM downloads](http://img.shields.io/npm/dm/@antv/g2plot.svg)](http://npmjs.com/@antv/g2plot)
![最近提交](https://badgen.net/github/last-commit/antvis/g2plot)


G2plot is an interactive and responsive charting library based on [the grammar of graphics](https://github.com/antvis/g2), which enables users to generate high quality stastical charts through a few lines of code easily. 

Moreover, combining with AntV design principles, g2plot provides standard and elegant visual styles as well as better user experience. 

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*MjhQQLsbWeQAAAAAAAAAAABkARQnAQ" width="200"><img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*CkSoSpPfWQMAAAAAAAAAAABkARQnAQ" width="200"><img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*ZYmtSqcNDtkAAAAAAAAAAABkARQnAQ" width="200"><img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*gV_JQZVbDWAAAAAAAAAAAABkARQnAQ" width="200">


## Installation

```
$ npm install @antv/g2plot
```

## Usage

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*37siRJftYDIAAAAAAAAAAABkARQnAQ" width="450">

```html
<div id="c1"></div>
```

```js
import g2plot from '@antv/g2plot';

const data = [
    {"year":"1951 年","sales":38},
    {"year":"1952 年","sales":52},
    {"year":"1956 年","sales":61},
    {"year":"1957 年","sales":145},
    {"year":"1958 年","sales":48}
  ];

const barPlot = new g2plot.Bar('c1', {
  data,
  xField: 'sales',
  yField: 'year',
  colorField: 'year'
});
        
barPlot.render();

```

## Development

```
$ npm install

# run test case
$ npm run test-live

# build watching file changes and run demos
$ npm run dev

# run demos
$ npm run demos
```

## How to Contribute

Please let us know how can we help. Do check out [issues](https://github.com/antvis/g2plot/issues) for bug reports or suggestions first.

To become a contributor, please follow our [contributing guide](https://github.com/antvis/g2plot/blob/master/CONTRIBUTING.md).



