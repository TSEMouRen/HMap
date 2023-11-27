### 鹰眼控件

> 使用视图映射作为其他定义的视图的概览图创建一个新的控件。

```javascript
  var Map = new HMap('map', {
    controls: {
      zoomSlider: false,
      zoom: false,
      rotate: false,
      overviewMap: true
    },
    view: {
      center: [12118909.300259633, 4086043.1061670054],
      zoom: 5,
    },
    baseLayers: [
      {
        layerName: 'openstreetmap',
        isDefault: true,
        layerType: 'OSM',
        layerUrl: 'https://{a-c}.tile.openstreetmap.org/{z}/{x}/{y}.png'
      }
    ]
  });
```

* ol.control.ScaleLineH 配置项说明

| 配置项 | 简介 | 类型 | 备注 |
| --- | --- |--- | --- |
| className | CSS类名，可自定义样式 | `String` | 非必传 默认使用封装好的 ```hmap-scale-line-control``` 样式 |
| minWidth | 容器宽度 | `Number` | 非必传 默认64|
| units	 | 单位 | `String` | 非必传 默认 'metric'|
| target | 控件的目标对象 | `Element` | 非必传 |
