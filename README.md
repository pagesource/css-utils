# CSS Utilities

## 1. Responisve Flex Grid
A responsive Flex box based grid Layouting module with SCSS and CSS3

## 2. Responsive 2 Dimensional Grid


_______

```css
<style>
    .container-fluid>.sn-flex {
      border: 1px solid #ccc;
      padding: 20px;
      margin: 20px;
    }

    .sn-flex>* {
      background-color: #eee;
      height: 50px;
    }
		.sn-flex>*:nth-child(even) {
    	background-color:#ccc;
		}

    .expend-height>.sn-flex {
      height: 200px;
    }

    h4 span {
      text-decoration: underline;
      font-weight: bold;
    }
</style>
```

```html
  <h1 class="sample-header">Flex Grid </h1>

  <div>
    <h4>The <span>sn-flex</span> class enables a flex context for all its direct children..

    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br/>
      &lt;div class="sn-flex"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br/>
      &lt;div class="sn-flex"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex">
      <div></div>
      <div></div>
    </div>
    <div class="sn-flex">
      <div></div>
      <div></div>
      <div></div>
    </div>
    <div class="sn-flex">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header" id="flex-3">{{page.fsdId}} - Grid Column</h1>
  <div>
    <h4>The <span>flex-</span> class to create columns i.e, to create 2 column use class column flex-2 for 3 column flex-3</h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-3"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br/>
      &lt;div class="sn-flex flex-4"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-3">
      <div></div>
      <div></div>
    </div>
    <div class="sn-flex flex-4">
      <div></div>
      <div></div>
    </div>
  </div>


  <h1 class="sample-header" id="flex-stack-mobile">{{page.fsdId}} - Small View Port Flex Overwrite</h1>
  <div>
    <h4>The <span>flex-stack-mobile</span> class to stack/Flex Overwrite all child element in mobile view</h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-stack-mobile"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-stack-mobile">
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid column Overwrite</h1>
  <div>
    <h4>The <span>grid-flex-overwrite</span> class to stack/Flex Overwrite columns, for this one more class required on child
      elemnet flex-overwrite</h4>
    <pre>
    <code>
      &lt;div class="sn-flex grid-flex-overwrite flex-3"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div class="flex-overwrite"&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex grid-flex-overwrite flex-3">
      <div></div>
      <div></div>
      <div class="flex-overwrite"></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Justify-content (Horizontally)</h1>
  <div>
    <h4>The <span>item-justify</span> class defines how the browser distributes space between and around content items along
      the main axis of their container.
      <br />
      <span>item-justify-</span>: start | end | center | between | around;
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-3 item-justify-left"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    <br />
      &lt;div class="sn-flex flex-3 item-justify-right"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br />
      &lt;div class="sn-flex flex-3 item-justify-center"&gt;
        &lt;div &gt;&lt;/div&gt;
        &lt;div &gt;&lt;/div&gt;
      &lt;/div&gt;
      <br />
      &lt;div class="sn-flex flex-3 item-justify-between"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br />
      &lt;div class="sn-flex flex-3 item-justify-around"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <h2>Justify left</h2>
    <div class="sn-flex flex-3 item-justify-left">
      <div></div>
      <div></div>
    </div>
    <h2>Justify right</h2>
    <div class="sn-flex flex-3 item-justify-right">
      <div></div>
      <div></div>
    </div>
    <h2>Justify center</h2>
    <div class="sn-flex flex-3 item-justify-center">
      <div></div>
      <div></div>
    </div>
    <h2>Justify between</h2>
    <div class="sn-flex flex-3 item-justify-between">
      <div></div>
      <div></div>
    </div>
    <h2>Justify around</h2>
    <div class="sn-flex flex-3 item-justify-around">
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Align Items (Vertically)</h1>
  <div class="expend-height">
    <h4>The <span>item-align-</span> class defines how the browser distributes space between and around content items along the
      main axis of their container.
      <br />
      <span>item-align-</span>: start | end | center | between | around;
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-3 item-align-start"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br />
      &lt;div class="sn-flex flex-3 item-align-end"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br />
      &lt;div class="sn-flex flex-3 item-align-center"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      &lt;div class="sn-flex flex-3 item-align-between"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
      <br />
      &lt;div class="sn-flex flex-3 item-align-around"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <h2>Align start</h2>
    <div class="sn-flex flex-3 item-align-start">
      <div></div>
      <div></div>
    </div>
    <h2>Align end</h2>
    <div class="sn-flex flex-3 item-align-end">
      <div></div>
      <div></div>
    </div>
    <h2>Align center</h2>
    <div class="sn-flex flex-3 item-align-center">
      <div></div>
      <div></div>
    </div>
    <h2>Align between</h2>
    <div class="sn-flex flex-3 item-align-between">
      <div></div>
      <div></div>
    </div>
    <h2>Align around</h2>
    <div class="sn-flex flex-3 item-align-around">
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-1-2</h1>

  <div>
    <h4>
      The class <span>flex-1-1-2</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile/tablet and 2 column in deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-1-2"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-1-2">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-1-3</h1>

  <div>
    <h4>
      The class <span>flex-1-1-3</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile/tablet and 3 column in deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-1-3"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-1-3">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-2-2</h1>

  <div>
    <h4>
      The class <span>flex-1-2-2</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile and 2 column in tablet/deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-2-2"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-2-2">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-2-3</h1>

  <div>
    <h4>
      The class <span>flex-1-2-3</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile, 2 column in tablet and 3 column in deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-2-3"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-2-3">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-3-3</h1>

  <div>
    <h4>
      The class <span>flex-1-3-3</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile and 3 column in tablet/deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-3-3"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-3-3">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-1-4</h1>

  <div>
    <h4>
      The class <span>flex-1-1-4</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile/tablet and 4 column in deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-1-4"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-1-4">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-2-4</h1>

  <div>
    <h4>
      The class <span>flex-1-2-4</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile, 2 column in tablet and 4 column in deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-2-4"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-2-4">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-3-4</h1>

  <div>
    <h4>
      The class <span>flex-1-3-4</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile, 3 column in tablet and 4 column in deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-3-4"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-3-4">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <h1 class="sample-header">{{page.fsdId}} - Flex Grid 1-4-4</h1>

  <div>
    <h4>
      The class <span>flex-1-4-4</span> use to get a three various-width columns starting at mobile and scaling to desktops
      <br/> 1 column in mobile and 4 column in tablet/deskop
    </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-1-4-4"&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
        &lt;div&gt;&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-1-4-4">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>


  <h1 class="sample-header">{{page.fsdId}} - Flex Grid as per content width</h1>

  <div>
    <h4>Use <span>flex-none</span> class to make container inline(width according to the content) </h4>
    <pre>
    <code>
      &lt;div class="sn-flex flex-none"&gt;
        &lt;div&gt;Component A&lt;/div&gt;
        &lt;div&gt;Component B&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex flex-none">
      <div>Component A</div>
      <div>Component B</div>
    </div>
  </div>


  <h1 class="sample-header">{{page.fsdId}} - Flex Grid grow classes</h1>

  <div>
    <h4>The <span>grow</span> class specifies how much the item will grow relative to the rest of the flexible items inside the
      same container.</h4>
    <pre>
    <code>
      &lt;div class="sn-flex grow"&gt;
        &lt;div&gt;Col 1&lt;/div&gt;
        &lt;div class="grow-2"&gt;Col 2&lt;/div&gt;
        &lt;div&gt;Col 3&lt;/div&gt;
        &lt;div class="grow-2"&gt;Col 4&lt;/div&gt;
        &lt;div&gt;Col 2&lt;/div&gt;
      &lt;/div&gt;
    </code>
  </pre>
    <div class="sn-flex grow">
      <div>Col 1</div>
      <div class="grow-2">Col 2</div>
      <div>Col 3</div>
      <div class="grow-2">Col 4</div>
      <div>Col 2</div>
    </div>
  </div>
</div>
```
