# Frontend Interview Challenge

Welcome!

Here you will find a set of problems to solve. These problems represent real-world scenarios you might encounter while working at Sandvine.

## Getting Started

### Pre-requisites

- NodeJS version 8+ [Download here](https://nodejs.org/en/)

Once node is installed clone this repository. Please ensure all work is done on a new feature branch:
```
git checkout -b sandvine-challenge-solutions
```

```
npm install
```

## Challenges

The challenges are broken into two groups - functional programming challenges and UI component challenges.

Challenges can be found in the `challenges/` directory. Each challenge contains three files:

#### `challenge.js`

This is where you will implement the function, or component, to complete the challenge. The contents of this file are entirely up to you, the only requirement is that the function signature remains the same and remains exported.

#### `data.json`

This contains the mock data that will be used for the particular challenge. These are made up events, or multiple groups of events, depending on the challenge.

#### `test.js`

Each challenge has a test file to verify the output for a series of inputs. Tests can be ran as they would in any standard node package.

### Meeting Availability Challenge

Find the available time slots within a given schedule.

```js
findFreeTimes(start: Date, end: Date, duration: number, events: Array<Event>)
```

[View the challenge](https://github.com/jean1880/frontend-interview-challenge/tree/master/challenges/1.%20Meeting%20Availability)

### User Availability Challenge

Find the available time slots that are free across a set of individual schedules.

```js
findFreeTimesAcrossSchedules(start: Date, end: Date, duration: number, schedules: Array<Array<Event>>)
```

[View the challenge](https://github.com/jean1880/frontend-interview-challenge/tree/master/challenges/2.%20User%20Availability)

### Component Challenge

Create a React or Angular component representing a common UI element seen across Sandvine.

```jsx
<AvailabilityTimePills
  start={startTime}
  end={endTime}
  duration={30}
  events={events}
/>
```

<img width="1000" alt="screen shot 2017-03-21 at 4 34 59 pm" src="https://cloud.githubusercontent.com/assets/656630/24169546/5e2610b6-0e54-11e7-87cd-0b70744dc269.png">


[View the challenge](https://github.com/jean1880/frontend-interview-challenge/tree/master/challenges/3.%20React%20Components)

## Preparing and submitting the challenge

Please submit your response in the form of a git patch. This can be generated by running the following command. Please check to make sure all your changes are committed before generating the patch file.

```
git format-patch master --stdout > <yourname>-solutions.patch
```

We look forward to seeing your solutions!
