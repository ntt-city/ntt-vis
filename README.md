# ntt-vis
Visualization is the way to communicate complex data.

## Charting https://youtu.be/qqffsEHKMcM

* Visual Analytics Machine Learning
* fancy-charts: rubbish
* composable charting
* victory charts
* react-vis
* recharts
* Taxonomic APIs

### The Grammar of Graphics (Leland Wilkinsons)

* Mark/Chart : Word/Language

* shapes (draw)
* scales (map data to view dimension)
* coordinate systems (to draw shapes into)
* axis, legend (guide components to know what you are looking at)
* data transformation components (aggregation, statistics, layout computation)

- Program Specification > Abstract Syntax Tree > Assembly

### Vega is a visualization grammar, a declarative language for creating, saving, and sharing interactive visualization designs. With Vega, you can describe the visual appearance and interactive behavior of a visualization in a JSON format, and generate web-based views using Canvas or SVG.

https://vega.github.io/vega/

* $schema: root starts with some props for scene nodes
* data: dada tables, each has a name, it can have a remote url and define a data model
* signals: event handling: internal signaling system. Singals are named variables that charts combine to and update in response to interactions, kind of a declarative redux.
* scales: is how we map data dimensions to ui dimensions such as which type of color. Each scale is a Named Object so we can reference them later.
* axes: oriented to the view space.
* marks: Visual components, shapes


### From Vega Abstraction to a React Component Based library (React): chart-parts

React Renderless >| Scene Builder > Abstract Scenegraph > Virtual SVG |> React-DOM

* areaTitle
* areaDescription

#### Other Charts

* PopulationChart

### React Native SVG Renderer

```js
import { Renderer } from '@chart-parts/react-native-svg-renderer';
const renderer = new Renderer();
const dataset = require('./data.json';

export default () => (
  <Chart renderer={renderer}>
  ...
  </Chart>
);
```
