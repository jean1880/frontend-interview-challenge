### React Components

The goal of this challenge is to create a React component for a range of "availability time pills", as well as the wrapping card with input fields:

<img width="1000" alt="screen shot 2017-03-21 at 4 34 59 pm" src="https://cloud.githubusercontent.com/assets/656630/24169546/5e2610b6-0e54-11e7-87cd-0b70744dc269.png">

The form should show:

 - A fixed date of "March 22, 2017"
 - A dropdown time selector
 - a dropdown duration selector

If the user selects an unavailable time slot, the pills should turn a reddish colour, and an error message should display notifying the user of the conflict. Add [Reactstrap](http://reactstrap.github.io/), and necessary dependencies to the project dependencies, and utilize provided components to quickly prototype the component, and keep custom CSS to a minimum.

Sample output of pill section:

```js
<TimeAvailabilityPills
  start={startOfTimeRange}
  end={endOfTimeRange}
  duration={timeRangeOfEachPill}
  events={collectionOfEvents}
/>
```

Which would output

```html
<div class="time-availability-pills">
  <div class="pill available">
    8:00am
  </div>
  <div class="pill available">
    8:30am
  </div>
  <div class="pill unavailable">
    9:00am
  </div>
  <div class="pill unavailable">
    9:30am
  </div>
  <div class="pill available">
    10:00am
  </div>
  <div class="pill available">
    10:30am
  </div>
</div>
```
