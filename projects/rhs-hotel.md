---
layout: project
type: project
image: img/rhs-hotel/rhs-hotel-thumbnail.png
title: "RHS Hotel Project"
date: 2018
published: true
labels:
  - HTML
  - CSS
  - JS
summary: "A small project that I worked on in high school that implemented a simple page for a 6 room hotel."
---

<div class="text-center p-4">
  <img height="200px" src="../img/rhs-hotel/rhs-hotel.png" class="img-thumbnail" >
</div>

Back when I was in high school beginning to learn about HTML, CSS, and JS, and how they can be used together, our teacher assigned us a project to create a sample page that a hotel might use. The page includes six rooms with individual guest lists of who is currently residing in each room, the ability to add and remove guests, lock and unlock the room to prevent new guests from checking in, and an overall guest log of all guests who have checked into the hotel, even if they have left already.

I was the only contributor to this project, as it was up to each individual to create their own hotel page based on what we were learning about in class, and applying the concepts to a semi-real-life example. I was responsible for figuring out how to program each function and operation that a standard hotel log might include, such as room guest lists, adding and removing guests from rooms (checking in and out), locking rooms so that no one else can enter or book on top of the existing members, checking out all guests from a certain room, and a total guest log of anyone that has checked into the hotel ever, regardless of room number.

From this project I learned how to map certain script functions from JavaScript to an HTML page, use CSS to stylize certain HTML elements of a web page, how to display a pop-up window when a button is clicked, and how to manage dates and lists in JavaScript. I also learned one of the basic skills of changing an HTML element's value dynamically, based on a user's actions or input. All of the JS functions that I used for each room can be found below: 

```cpp
      function oneName() {
        var currentDate = new Date();
        var date = currentDate.getDate();
        var month = currentDate.getMonth();
        var year = currentDate.getFullYear();
        var n = currentDate.toLocaleTimeString();
        var dateString = (month + 1) + "/" + date + "/" + year;
        if (onePpl.value !== "" && rmoneAmount < 4) {
        rmoneAmount++;
        var oneppl = document.getElementById('onePpl').value;
        allRooms.push(oneppl);
        document.getElementById('onePpl').value = "";
        var ol = document.getElementsByTagName('ol')[0];
        var newLi = document.createElement('li');
        var newText = document.createTextNode(oneppl + " " + dateString + " " + n);
        newLi.appendChild(newText);
        ol.appendChild(newLi);
        document.rmOne.appendChild(ol);
        }
        else if (onePpl.value !== "" && rmoneAmount > 3) {
          window.alert("Room is full");
        }
      }
      
      function onePer() {
        var oneNum = document.getElementById('oneNum').value;
        var getLi = document.getElementsByTagName('li')[oneNum - 1];
        var getParent = getLi.parentNode;
        getParent.removeChild(getLi);
        rmoneAmount--;
      }
      
      function oneLock() {
        document.getElementById('onePpl').disabled = true;
        document.getElementById('oneName').disabled = true;
        document.getElementById('oneNum').disabled = true;
        document.getElementById('onePer').disabled = true;
        document.getElementById('oneAll').disabled = true;
        document.getElementById('oneLock').disabled = true;
      }
      
      function oneUnlock() {
        document.getElementById('onePpl').disabled = false;
        document.getElementById('oneName').disabled = false;
        document.getElementById('oneNum').disabled = false;
        document.getElementById('onePer').disabled = false;
        document.getElementById('oneAll').disabled = false;
        document.getElementById('oneLock').disabled = false;
      }
      
      function oneAll() {
        document.getElementById('unoppl').innerHTML = "";
        rmoneAmount = 0;
      }
```

Source: <a href="https://github.com/isaseg/hotel-project">isaseg/hotel</a>
