# Project Overview
Yexenia Flores
## Project Name

T & D 

## Project Description

This will be a Tappas and Drinks app where the person can find a drink that they wish to make. The second part will be for them to get a random tappas or snack that they can make so it can go along with their drink. 

## API and Data Sample

I am using two API's for my app, the first one is for making cocktails (https://www.thecocktaildb.com/api.php), I will be setting it up so the user can search by name.  

![Screen Shot 2021-12-12 at 10 15 31 PM](https://user-images.githubusercontent.com/92563217/145749506-970b5812-7aca-416f-9526-7c9c6cee5333.png)

The Second one will be ( https://developer.edamam.com/) so it can give a random snack that can go with their drink that they looked up. 

![Screen Shot 2021-12-12 at 10 15 31 PM](https://user-images.githubusercontent.com/92563217/145749590-0419858f-ff58-4dbd-99cc-9ec64e670828.png)

## Wireframes

Upload images of your wireframes to an image hosting site or add them to an assets folder in your repo and link them here with a description of each specific wireframe.

Mobile

<img width="261" alt="Screen Shot 2021-12-12 at 10 22 18 PM" src="https://user-images.githubusercontent.com/92563217/145753706-dee2c685-4f9e-4ae7-a65b-4dec5e90fed1.png">

Window

<img width="878" alt="Screen Shot 2021-12-13 at 9 18 10 AM" src="https://user-images.githubusercontent.com/92563217/145828746-b0fb5381-d767-4974-868d-8c5ed16f8355.png">


### MVP/PostMVP


#### MVP 
*These are examples only. Replace with your own MVP features.*

- Generate the cocoktail that the person is going to search for 
- Lay out the name, ingredients, and steps to make the drink
- Post the image of the drink
- Generate a random snack that they can make
- Display the ingredients of the snack 
- Post the image of the snack

#### PostMVP  
*These are examples only. Replace with your own Post-MVP features.*

- Add dropdown menu to see cocktails by liquor
- Add search for specific snack user wants to make
- create a more creative design to the app 
- Use local storage to save user favorites

## Project Schedule

This schedule will be used to keep track of your progress throughout the week and align with our expectations.  

You are **responsible** for scheduling time with your squad to seek approval for each deliverable by the end of the corresponding day, excluding `Saturday` and `Sunday`.

|  Day | Deliverable | Status
|---|---| ---|
|Dec 10-12| Prompt / Wireframes / Priority Matrix / Timeframes | Complete
|Dec 13| Project Approval | Complete
|Dec 13| Core Application Structure (HTML, CSS, etc.) | Complete
|Dec 14| Pseudocode / actual code | Complete
|Dec 15| Initial Clickable Model  | Complete
|Dec 16| MVP | Complete
|Dec 17| Presentations | Incomplete

## Priority Matrix

<img width="801" alt="Screen Shot 2021-12-12 at 11 12 30 PM" src="https://user-images.githubusercontent.com/92563217/145751656-53701f08-d791-42da-b1b9-c8a10441fec0.png">

## Timeframes

Tell us how long you anticipate spending on each area of development. Be sure to consider how many hours a day you plan to be coding and how many days you have available until presentation day.

Time frames are also key in the development cycle.  You have limited time to code all phases of the game.  Your estimates can then be used to evalute game possibilities based on time needed and the actual time you have before game must be submitted. It's always best to pad the time by a few hours so that you account for the unknown so add and additional hour or two to each component to play it safe. Throughout your project, keep track of your Time Invested and Actual Time and update your README regularly.

| Component | Priority | Estimated Time | Time Invested | Actual Time |
| --- | :---: |  :---: | :---: | :---: |
| HTML | H | 3hrs| 3hrs | 3hrs |
| CSS | H | 3hrs| 4.5hr | 4.5hrs |
| JAVASCRIPT | H | 4hrs| 7hrs | 7hr |
| API | H |2hrs| 3hrs | 3hrs |
|LAYOUT| H | 4hrs| 4hrs | 4hrs |
|IMAGES| H | 4hrs| 3hrs | 3hrs |
|DEBUGGING| H | 3hrs | 3.5 hrs | 3.5hrs |
| DATA CONNECTION | H | 6hrs| 7hrs | 7hrs |
| CCS DESIGN | H | 5hrs| 4.5hrs | 4.5hrs |
| ADVANCE DEGISN | L | 1hr| 1hr | 1hr |
| MORE BUTTONS| M | 1hr| 0hrs| 0hrs |
| TESTING| H | 3hrs | 4.5 hrs | 4.5 hrs |
|POSTMVP| L | 3hrs | 1hr | 1hr |
| Total | H | 45hrs| 46hrs | 46hrs |

## Code Snippet

I am proud of this code snippet that Shay helped me on because despite the complexity of it, I understood what it is doing. Because my ingredients and measurements were in different keys, I had to loop through the array twice in order to get them in the same line.  

```
 for (const [key, value] of Object.entries(drink)) {
      if (key.includes("strIngredient")) {
        if (value) {
          const num = key.split('strIngredient')
          const h3 = document.createElement("h3")
          if (drink[`strMeasure${num[1]}`]) {
            h3.innerText = `${drink[`strMeasure${num[1]}`]} ${value}`
          } else {
           h3.innerText = value
          }
          div.appendChild(h3)
        }
      } 
     }
```

## Change Log
 Use this section to document what changes were made and the reasoning behind those changes.  
