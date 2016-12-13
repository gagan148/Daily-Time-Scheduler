# Daily-Time-Scheduler
### How to use it:

1. Include the needed jQuery and jQuery UI on the html page.

```javascript
<script src="jquery.min.js"></script>
<script src="jquery-ui.min.js"></script>
<link rel="stylesheet"href="jquery-ui.css">
```
2. Include the jQuery schedule plugin's stylesheet and JavaScript after jQuery library.

```javascript
<script src="jq.scheduler.js"></script>
<link rel="stylesheet" href="style.css">
```

3. Render a basic time schedule with custom events.

```javascript
jQuery("#schedule").timeSchedule({
  rows : {
    '1' : {
      title : 'Title Area',
      schedule:[{
        start:'09:00',
        end:'12:00',
        text:'Text Area',
        data:{}
      },{
        start:'11:00',
        end:'14:00',
        text:'Text Area',
        data:{}
      }]
    },},
});
```
4. Customization options.

```javascript
// scheduled events
rows: {},

// schedule start time(HH:ii)
startTime: "07:00",

// schedule end time(HH:ii)
endTime: "21:00", 

// width(px)
widthTimeX: 25,

// cell timestamp example 10 minutes
widthTime: 60 * 10, 

// height(px)
timeLineY: 60,   

// options for time slots
timeLineBorder: 1,
timeBorder: 1,   // border width
timeLinePaddingTop: 0,
timeLinePaddingBottom: 0,
headTimeBorder: 1, // time border width 

// data width
dataWidth: 160, 
```

5. Events
```javascript
init_data: null,
change: null,
click: null,
append: null,
time_click: null,
debug: ""      // debug selecter
```

### Stuff used to make this:

 * [jQuery](https://jquery.com/) 
 * [jQuery UI](https://jquery.com/) 
