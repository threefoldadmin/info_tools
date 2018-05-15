
# echart

```chart
{
  xAxis : [
    {
      type : 'category',
      data : ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
    }
  ],
  yAxis : [{ type : 'value' }],
  series : [
    {
      name:'sss',
      type:'bar',
      barWidth: '60%',
      data:[10, 52, 200, 334, 390, 330, 220]
    }
  ]
}
```

```chart
option = {
    xAxis: {
        type: 'category',
        boundaryGap: false,
        data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
    },
    yAxis: {
        type: 'value'
    },
    series: [{
        data: [820, 932, 901, 934, 1290, 1330, 1320],
        type: 'line',
        areaStyle: {}
    }]
};
```

- see http://echarts.baidu.com/
- - [examples](https://ecomfe.github.io/echarts-examples/public/)