

# CSS Grid

```js
<fieldset>
<h1>CSS Grid</h1>
<style>
   #cssGrid {
      display: grid;
      border: 2px blue solid;
      height: 500px;
      width:100%;
      grid-template: repeat(4, 1fr 2fr) / repeat(4, 3fr 2fr);
      grid-gap: 5px;
    }

    .cssGridBoxA {
      grid-area: 5 / span 2;
       1 / span 2;
    }

    .cssGridBoxB {
      grid-column: 2 / span 6;
      grid-row: 2 / span 3;
    }
    .cssGridBoxC {
      grid-area: 6 / 8 / span 3 / span 1;
    }
    .cssGridBox {
      background-color: beige;
      color: black;
      border-radius: 5px;
      border: 2px dodgerblue solid;
    }
</style>

<div id="cssGrid">
    <div class="cssGridBox cssGridBoxA">Box A</div>
    <div class="cssGridBox cssGridBoxB">Box B</div>
    <div class="cssGridBox cssGridBoxC">Box C</div>
</div>

</fieldset>
```