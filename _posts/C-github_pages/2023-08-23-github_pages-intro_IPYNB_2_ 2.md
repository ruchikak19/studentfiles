---
layout: post
title: GitHub Pages
description: The Web Programming topics are focused on learning Frontend programming, GitHub Pages, and Jupyter Notebooks.
categories: ['JavaScript']
permalink: /github/pages/intro
type: ccc
courses: {'csse': {'week': 2}, 'csp': {'week': 2}, 'csa': {'week': 1}}
author: John Mortensen
menu: nav/github_pages.html
---

## GitHub Pages Mini Project

Your Teacher wants you to engage in a mini project!  This project is intended to help you and your programming pair to make an information site.  The required topics for this mini project include ...

- Making a submenu
- Using the submenu headings to Guide sub topics
- Make your own customized pages for each submenu
- Create some data that will help you track information about your topic
- Make some submenu pages that perform actions through JavaScript
- Review the anatomy of GitHub pages
  - Review and experiment with the usage of Styles in GitHub Pages
Start the process of inspecting and debugging

## Topics

The topic for your mini project is up to you.
- Perhaps you wnat to make a submenu of your favorite games and inside each article you can capture data and talk about techniques to enhance place (list discord groups, list communities you have joined, share a list of key videos to enhance success, make a list of popular mods you have added, discuss properties of avatars, etc )  
- In fitness training you could make menus that highlight highlight topics and results by define a training regimine, track results/data on regimine, define key offline preparations (sleep, nutrition, water, calories, steps), etc


### Brainstorm

To brainstorm is often done by sharing or talking about topics with a pair.  In your project you will capture your brainstorm of your project.

- Gaming Blog
- Fitness Blog
- Raising Fish
- Career Humor

## Brainwrite 

The Teacher descited to create a mini project on Career Humor.  As a Brainwrite activity, the Teacher decided to think about careers that are possible pursuts of subjects taught at Del Norte High School.

### Brainwrite Submenu

My brainwrite took the brainstorm idea of **Career Humor** and established some categories.   

1. Computer Science
2. Accountant
3. Jounalism
4. Film and Media
5. Mechanical Engineer
6. Biomedical Engineer
7. Astronomer


### Brainwrite Data

Beyond initial categories, my brainwrite went into the direction of authoring joke data.  Amazingly, after some initial research on Computer Science, the Teacher found that ChatGPT could help with jokes on Accountings.

**Note** To observe outputs from Javascript **console.log**, open the Developer Tools
  - In VSCode, go to **Help->Toggle Developer Tools**
  - Click on **Console** in the newly opened Window
  - Clear screen by pressing **Clear Console** (circle with line)
  - Then press **Play button** to left of cell
  - Observer random output in Console


```javascript
%%javascript

var compsci_joke_list = [
    { joke: "Why do programmers prefer dark mode? Because light attracts bugs.", complexity: "O(1)" },
    { joke: "Why do Java developers wear glasses? Because they don't see sharp.", complexity: "O(1)" },
    { joke: "How many programmers does it take to change a light bulb? None, that's a hardware problem.", complexity: "O(1)" },
    { joke: "Why do programmers hate nature? It has too many bugs.", complexity: "O(n)" },
    { joke: "Why do Python programmers prefer snake_case? Because they can't C.", complexity: "O(1)" },
    { joke: "Why was the JavaScript developer sad? Because he didn't know how to 'null' his feelings.", complexity: "O(1)" },
    { joke: "Why do programmers always mix up Christmas and Halloween? Because Oct 31 == Dec 25.", complexity: "O(1)" },
    { joke: "Why did the programmer quit his job? Because he didn't get arrays.", complexity: "O(n)" },
    { joke: "Why do programmers prefer using the terminal? Because they don't like Windows.", complexity: "O(1)" },
    { joke: "Why was the function sad after a breakup? It couldn't find its closure.", complexity: "O(1)" }
];
var randomIndex = Math.floor(Math.random() * compsci_joke_list.length);
var selectedJoke = compsci_joke_list[randomIndex];
console.log("Joke #" + (randomIndex + 1) + ": " + selectedJoke.joke + " (Complexity: " + selectedJoke.complexity + ")");
```


    <IPython.core.display.Javascript object>



```javascript
%%javascript

var athlete_joke_list = [
    "Why did the basketball player bring a duck to practice? Because he wanted more quack-boards. 🏀🦆",

"Why did the golfer change his socks? Because he had a hole in one… and a blister in the other. ⛳🧦",

"Why don’t baseball players ever get hot? Because they have so many fans. ⚾🪭",

"Why did the sprinter apply for a job at the bakery? He was great at making things roll fast. 🏃‍♂️🥖",

"Why did the soccer team go to the bakery? Because they needed a good striker roll. ⚽🥐",

"Why did the football player bring string to the game? To tie the score. 🏈🪢",

"What do you call a polite tennis player? A real ace gentleman. 🎾🎩",

"Why did the hockey player break up with his girlfriend? She kept giving him the cold shoulder. 🏒🥶",

"Why don’t runners ever get locked out of their house? Because they always jog their memory. 🏃‍♀️🧠",

"Why did the weightlifter bring a ladder to the gym? Because he wanted to take his reps to the next level. 🏋️‍♂️🪜"
]
var randomIndex = Math.floor(Math.random() * athlete_joke_list.length);
console.log("Joke #" + (randomIndex + 1) + ": " + athlete_joke_list[randomIndex]);
```


    <IPython.core.display.Javascript object>


## Mini Project Files

Learning how to manage files in GitHub Pages is a key skill.  This class will continually share files and have challenges using GitHup Pages and Jupyter Notebooks.  Even though you will be working as a pair, you will need to share files with your partner.
- Each pair will have their own GitHub Pages repository with their own files.
- To copy files between repostories, 
  - **git clone** both repositories, yours and your pairs
  - **git pull** keeps repostitories up to date, mostly you will need to do this on your pairs
  - **code .** in directory you cloned will open vscode windows 
  - **drag and drop** files between repositories, be sure to put them in correct folders

### Key Locations for this mini Project

- The **_includes** directory is a location to place files that you want to share across many notebooks.  
  - In this directory on porfolio_2025 you submenu files.
  - The location **_includes/nav/github_pages.html** is a shared submenu
  - Inside the file you will see tags: **table**, **tr** (table row), **td** (table data), and **a** (link) 

- The **_notebooks** directory is the default location to place all **.ipynb** files.  This is the location for all interactive notebooks in our GitHub Pages projects.  If files are in the location they are converted to Web Pages through GitHub Pages Actions.
  - For starters you could copy **_notebooks/Foundation/C-github_pages** to your project.
  - Then you could rename or make modification to thes files as required.


- The **_notebooks/Foundations/C-github_pages** contains the files that use the submenu
  - In **frontmatter** of each file you will 
    - **menu: nav/github_pages.html** the menu (submenu) that is included for the page
    - **permalink: /github/pages/intro** the reference for this pages that corresponds to **a** tage in in submenu table



