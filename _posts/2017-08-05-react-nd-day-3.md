---
published: false
title: 'React ND - Day #3'
categories:
  - udacity
  - react
tags:
  - udacity
  - react
  - lessons
---
## Day #3
* Worked from 3:43am - 4am
* Made it through Lesson 4

### Lesson 4: Rendering UI with External Data
Nothing special in this lesson. It took about 40 minutes to complete. It introduced React's **Lifecycle Events**.

#### Lifecycle Events
These are special methods each React component has that allows us to tap into different points in its life to manipulate state. We can breakdown these methods into three different points: 
1. Adding to the DOM
2. Re-rendering the DOM
3. Removing from the DOM

Another visual: 
![React Lifecycle Events]({{site.baseurl}}/images/react-lifecycle-events.png)

Is it obvious that I'm a visual learner? 😝

The most commonly used lifecycle event is the `componentDidMount()` method. This method runs immediately after the components is added to the DOM. So, this would be a great place to make AJAX calls, i.e. retrieving data from our backend server. However, be careful calling `setState()` in this method! Setting state will cause the component to re-rendering. This might throw you into a loop!

### Takeaway
I use the `componentDidMount()` method a lot! Probably, the majority of time I need to manipulate my component state. Now that I'm aware of all these other lifecycle events and their purpose, I can use them properly in my projects. 