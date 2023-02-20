# coffee-masters
building an checkout page for a coffee app using grid 

# Overlayed Input


```html
<div class="example-group">
  <label for="example" class="input-label">Example Text</label>
  <input id="example" class="example-input" placeholder="try typing here" />
</div>
```
```css
  .example-group {
    position: relative;
    display: inline-block;
  }

  .example-input {
    border-color: crimson;
    padding: 8px;
    border-radius: 5px;
  }

  .input-label {
    background-color: white;
    color: crimson;
    font-size: 11px;
    position: absolute;
    left: 25px;
    top: -7px;
    padding: 0 2px;
  }
```


## Result:
Just a quick example to show you how to overlay a label over an input's border

- We're using a containing div with position: relative set on it. This is so the position: absolute of the input label is absolute relative to to the containing div, and not the whole page. Try taking off the relative position of the container and watch the label fly somewhere else.


- Labels allow users to click on the label and have that click select the input. Hence the for="" attribute and how it matches the id of the input.


- I then just eyeballed the best left and top values to use


