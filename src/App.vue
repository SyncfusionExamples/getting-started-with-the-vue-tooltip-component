<script setup>
import { TooltipComponent as EjsTooltip } from "@syncfusion/ej2-vue-popups";
import { ButtonComponent as EjsButton } from "@syncfusion/ej2-vue-buttons";
</script>

<template>
<ejs-tooltip target="#target" :content="'contentTemplate'" position="RightCenter"
             isSticky="true">
    <template v-slot:contentTemplate>
      <div id='democontent' ref="content">
        <div className='info'>
          <h3>Eastern Bluebird</h3>
          <div>
            <div>
                The<a href='https://en.wikipedia.org/wiki/Eastern_bluebird' target='blank'> Eastern Bluebird</a>
                is easily found in open fields and sparse woodland areas, including along woodland edges.These are<i>cavity-nesting birds</i>and a pair of eastern bluebirds will raise 2-3 broods annually, with 2-8 light blue or whitish eggs per brood.
            </div>
            <div id='bird'>
              <img src='https://ej2.syncfusion.com/react/demos/src/tooltip/images/bird.png' width='250' height='170' style="padding-left:69px; padding-top:20px;" /></div>
          </div>
          <div>
              <p> Eastern bluebirds can be very vocal in flocks. Their calls include a rapid, mid-tone chatter and several long dropping pitch calls.</p>
          </div>
        </div>
      </div>
    </template>
    <div id="container">
        <ejs-button id="target">Show Tooltip</ejs-button>
    </div>
</ejs-tooltip>
</template>

<style>
 @import "../node_modules/@syncfusion/ej2-base/styles/material.css";
 @import "../node_modules/@syncfusion/ej2-vue-buttons/styles/material.css";
 @import "../node_modules/@syncfusion/ej2-vue-popups/styles/material.css";
 #container {
    display: inline-block;
    position: relative;
    left: 60%;   
    transform: translateX(-50%);
    height: 200px;
    margin-top: 10px;
  }

  #target {
    display: inline-block;
    margin: 30px 130px 30px 50px;
  }

</style>
