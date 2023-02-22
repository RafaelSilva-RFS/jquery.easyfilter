# jQuery EasyFilter
The easiest way to filter anything!
Check the [live demo and documentation](https://rafaelsilva-rfs.github.io/jquery.easyfilter/)

## How to use

#### 1. Include jQuery (ignore this if you have already included on the page).
```html
<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
```

#### 2. Include jQuery EasyFilter plugin.
```html
<script src="./js/jquery.easyFilter.min.js" type="text/javascript"></script>
```

#### 3. Create the markup, you will need a `container` where you will put elements with `data-easyfilter` attribute that have the Click Listener Event and elements with `data-easyitem` attribute that will be filtered.
```html
<div id="easy-filter-wrap">
     <button type="button" data-easyfilter="*"> All </button>
     <button type="button" data-easyfilter="item01,item02"> Item 01 and 02 </button>
     <button type="button" data-easyfilter="item01"> Item 01 </button>
     <button type="button" data-easyfilter="item02"> Item 02 </button>
     <button type="button" data-easyfilter="item03"> Item 03 </button>
     <br /> <br />
     <div data-easyitem="item01"> Item 01 </div>
     <div data-easyitem="item02"> Item 02 </div>
     <div data-easyitem="item03"> Item 03 </div>
</div>
```

#### 4. Initialize the EasyFilter plugin.
```html
<script>
     $('#easy-filter-wrap').easyFilter();
</script>
```

## Options
```javascript
$('#easy-filter-wrap').easyFilter({
    firstFilter: '*',
    animation: 'slide',
    duration: 400
});
```

| Option | Type | Description |
| --- | --- | --- |
| `firstFilter` | string | Default: `'*'`. <br> Controls the first elements to show. |
| `animation` | string | Default: `'slide'`. <br> Select the animation. <br> Values: `'slide'` \| `'fade'` |
| `duration` | int \| string | Default: `400`. <br> Controls the animation duration. <br> Values: `'slow'` \| `'normal'` \| `'fast'` \| `Any integer` |

## License
[MIT License](https://github.com/RafaelSilva-RFS/jquery.easyfilter/blob/master/LICENSE)