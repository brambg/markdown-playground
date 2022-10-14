# markdown-playground
Play around with GH MarkDown features

<!-- this will get processed correctly in the gh-pages view -->
<style>

/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
}

/* Style the buttons that are used to open the tab content */
.tab button {
  background-color: inherit;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}

</style>

<script>
function openCity(evt, cityName) {
  // Declare all variables
  var i, tabcontent, tablinks;

  // Get all elements with class="tabcontent" and hide them
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }

  // Get all elements with class="tablinks" and remove the class "active"
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }

  // Show the current tab, and add an "active" class to the button that opened the tab
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>

<table>
<tr><td>A</td><td>B</td></tr>
<tr><td>C</td><td>D</td></tr>
</table>

<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'kotlin-1')">Kotlin</button>
  <button class="tablinks" onclick="openCity(event, 'java-1')">Java</button>
</div>

<div id="kotlin-1" class="tabcontent">
  <h3>Kotlin</h3>
  <p>Kotlin is a programming language with limited overhead</p>
</div>

<div id="java-1" class="tabcontent">
  <h3>Java</h3>
  <p>Java is a programming language with a lot of overhead</p>
</div>

<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'kotlin-2')">Kotlin</button>
  <button class="tablinks" onclick="openCity(event, 'java-2')">Java</button>
</div>

<div id="kotlin-2" class="tabcontent">
  <h3>Hello World</h3>
  <p>
    ```kotlin
    println("Hello World")
    ```
  </p>
</div>
    ```kotlin
    println("Hello World")
    ```

<div id="java-2" class="tabcontent">
  <h3>Hello World</h3>
```java
system.out.println("Hello World");
```
</div>
```java
system.out.println("Hello World");
```


_Kotlin_
```kotlin
println("Hello World")
```

#### Java
```java
system.out.println("Hello World");
```
