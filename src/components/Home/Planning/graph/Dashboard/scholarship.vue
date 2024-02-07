<template>
    
    <v-chart class="chart" :option="option" autoresize />
    
  </template>
  
  <script setup>
  import { use } from 'echarts/core';
  import { CanvasRenderer } from 'echarts/renderers';
  import { PieChart } from 'echarts/charts';
  import {
    TitleComponent,
    TooltipComponent,
    LegendComponent,
  } from 'echarts/components';
  import VChart, { THEME_KEY } from 'vue-echarts';
  import { ref, provide } from 'vue';
  
  use([
    CanvasRenderer,
    PieChart,
    TitleComponent,
    TooltipComponent,
    LegendComponent,
  ]);
  
  provide(THEME_KEY, 'white');
  
  const option = {
  
  title: {
    text: 'Scholarship',
    left: '0',
    bottom:'50%'
  },
  label:{
    show:true,
    formatter(param){
        return param.name + '('+param.percent  + '%)';
    }
  },
  tooltip: {
    trigger: 'item'
  },
  legend: {
    orient: 'vertical',
    left: 'left'
  },  color:[

    "#EC061D",
    "#06ECC3",
  ],
  series: [
    {
      name: 'Access From',
      type: 'pie',
      radius: '70%',
      data: [
        { value: 1048, name: 'Internally Funded' },
        { value: 195, name: 'Externally Funded' },

      ],
      emphasis: {
        itemStyle: {
          shadowBlur: 10,
          shadowOffsetX: 0,
          shadowColor: 'rgba(0, 0, 0, 0.5)'
        }
      }
    }
  ]
};

  </script>
  
  <style scoped>
  .chart {

    height: 55vh;
    width: 80%;
   
  }
  </style>
  