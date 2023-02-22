# Lecture Reference: DOM Manipulation #####################

# What is the DOM?
    # - stands for Document Object Model
    # - it's a layer between the html source and what the browser displays
    # - you use JS to interact with it
    # - when you modify the DOM, the source HTML stays the same 
    # - console.log(document) --> you can see what document looks like in 
    # browser console and expand it (it's a JS object)
    # - helps JS and HTML work together to make webpage interactive
    # - shaped like a tree just like the html

# What do we mean when we say the DOM is a tree?
    # nested
    # like a family tree (parents, children, siblings)

# How do we select DOM elements?
# a single element:
    const frog = document.getElementById("frog")
    const bunny = document.getElementById("bunny")
    const queryFrog = document.querySelector("#frog")
    console.log(queryFrog)
    
# multiple elements
    const classAnimal = document.querySelectorAll(".animal")
    console.log(classAnimal)

# How do we create DOM elements?
    # 1. identify parent element
        const animalList = document.getElementById("animal-list")
    # 2. create new DOM element, save to variable
        const cat = document.createElement("li")
        const elephant = document.createElement("li")
        cat.textContent = "cat"
        elephant.textContent = "elephant"
    # 3. append new dom element
        # the format is parent.append(child1, child2 (optional)...)
        animalList.append(cat, elephant)

# How do we change DOM elements?
    bunny.textContent = "tiger"

# How do we remove DOM elements?
    bunny.remove()