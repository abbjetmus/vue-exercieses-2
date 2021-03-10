# vue-exercieses
Start by cloning the project at:
<br>
`git clone https://github.com/abbjetmus/vue-exercieses-2.git`
<br>
## To think about

1. Use back-ticks **\` \` (shift + `)** if you want html over multiple rows.
```
var testcomponent = {
       template: `
           <div>
              <p></p>
           </div>
          `
       }
```
2.	Use small letters on component-name and events/methods.

## Question 1 - Interpolation

Create two data variables called **pi** and **e**, assign pi the value 3.14 and e the value 2.71. <br>
Then print the text **"Pi has the value 3.14"** and **"E has the value 2.71"** using the data variables and optional tags.

### Result
**Pi has the value 3.14**<br><br>
**E has the value 2.71**<br>

## Question 2 - Looping
1. Create a data variable named **students** which is a **array []** and contains three objects with students:

```
{id: 1, name: 'Kalle'},
{id: 2, name: 'Pelle'},
{id: 3, name: 'Nalle'}
```

2. Then loop through the array of students in an html list where you print the name, <br>
you choose whether you want to use <**ul**> unorderd-list or <**ol**> ordered-list.

### Result
* Kalle
* Pelle
* Nalle

## Question 3 – Two-way-bindning

1. Create an input field with the **input** tag.
2. The field should be two-way-bound using **v-model** to a data variable called image.
Create an <img> tag that also binds to the image variable with the src attribute and displays the image that is entered into the input tag.
4. Google any image and copy the image address to the input field so that it appears in the <img> tag.

### Result
![](./assets/uppgift3.gif)

## Question 4 – Watchers 
Create a data variable named **politician** which is a **array []** and contains five objects with politicians:
```
{id: 1, firstName: 'Stefan', lastName: 'Löven'},
{id: 2, firstName: 'Annie', lastName: 'Lööv'},
{id: 3, firstName: 'Nyamko', lastName: 'Sabuni'},
{id: 4, firstName: 'Jimmie', lastName: 'Åkesson'},
{id: 5, firstName: 'Per', lastName: 'Bolund'},
```

2. Create an input field with the **input** tag.
The field should be able to take in a number and two-way bind using v-model to a data variable called **selectedId**.
4. Create another variable named **selectedPolitician**.
5. Then create a **watcher** that listens to the value in selectedId and based on selectedId, politicians filter the array after the politician with that **id**.
Use the JavaScript **find** function: <https://www.w3schools.com/jsref/jsref_find.asp>
selectedPolitician must be assigned to the filtered politician in the watch.
6. Display the name of the selectedPolitician with any tag in the html code.

### Result
![](./assets/uppgift4.gif)

## Question 5 – Class bindning (Class binding)
Create a checkbox with the input tag that binds two-way with **v-model** to a data variable called **background** with the value **false**.
Then use two css classes in the styles tag inside the head tag called "backgroundGreen", and "backgroundRed".
```
    <style>
        .backgroundGreen {
            background-color: green;
        }

        .backgroundRed {
            background-color: red;
        }
    </style>
```
the classes must set background-color to red and green respectively.
3. Then create a div tag with the code below:
```
<div style="width: 200px; height: 200px;"></div>
```
4. Bind the div attribute's class attribute so that the background color changes between red and green when ticking in and out of it.
### Result
![](./assets/uppgift5.gif)

### Question 6 – Slots 
1. Create a component called **bodycomponent**.
2. **bodycomponent** shall have four named slots with the names "head", "shoulder", "knee" and "toe".
Then use **bodycomponent** in the '#app' component and submit four optional tags via the slots with the text
"Head, shoulders, knee and toe".

### Result

**Head**<br><br>
**Shoulders**<br><br>
**Knee**<br><br>
**Toe**<br><br>


## Question 7 – Component communication
1. Create a data variable named **politicianList** which is a **array[]** and contains five objects with politicians:
```
{id: 1, firstName: 'Stefan', lastName: 'Löven', party: 'Socialdemokraterna'},
{id: 2, firstName: 'Annie', lastName: 'Lööv', party: 'Centerpartiet'},
{id: 3, firstName: 'Nyamko', lastName: 'Sabuni', party: 'Liberalerna'},
{id: 4, firstName: 'Jimmie', lastName: 'Åkesson', party: 'Sverigedemokraterna'},
{id: 5, firstName: 'Per', lastName: 'Bolund', party: 'Mijlöpartiet'},
```

Also create a variable named **selectedPolitician**<br>

2. Then create a component called **politicianitem** that takes in a politician as a prop.
**politicianitem** shows the politician's name together with a button next to it. <br>
When the button is clicked, the politician should be sent to the parent component (the app component) and assigned to
selectedPolitician. <br>
4. **selectedPolitician** should then be displayed in html with all information.

### Result
![](./assets/uppgift6.gif)

## Question 8 – Life-cycle-hooks
1. Make an API call with the following fetch calls using the appropriate life-cycle method:

```
fetch('https://jsonplaceholder.typicode.com/photos/1')
  .then(response => response.json())
  .then(json => console.log(json))
```

2. Look at the data types in the browser console.
3. Then store the data in a variable called photo.
4. Present the photo in the html with appropriate tags.


### Result
![](./assets/uppgift8.png)

