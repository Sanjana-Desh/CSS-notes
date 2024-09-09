3 Different types of Selectors:
- element selector: which selects all the specified element
- class selector (.) : two or more elements can be selcted using class
- id selector (#): id's are unique no two elements have same id, avoid id selector keep them out of css

# Group slector
h1, h2{color:white;}
- the comma is used for separation

# nesting
p span{
    color:white;
}
- selects the span element inside the p tag and then colors them 

# universal
*{font-family: monospace;}
- selects everything

# ------------------------------------------------- SPECIFICITY ------------------------------------------- #

- css = cascading style sheet
- cascading = works like waterfall
- jo niche h wo display hoga

p{
    color:white;
}

p{
    color:black;
}

- it displays black
- class selector has more priority even if it is at top compared to element selector

.s1{
    color:white;
}

p{
    color:black;
}
- white is selected
- therefore more the specificity more the priority !important>id>class>element
.s1{
    color:white;
}

p{
    color:black!important;
}
- black is selected
- DO NOT USE THE IMPORTANT FLAG DOO NOT

# -------------------------------------------------------- Inheritance ---------------------------------------- #

- That is where the element inherits property from parent element

- anything realted to typography or font is inherited from parents to child

<body> <p> hello </p> </body>

- here if i use font to body it will apply to p also, but if i use border to body that wont apply to p as it is not font related
- it helps us in reducing code
- formed elements do not take inherit code to make them take it

button, input, textarea, select {
    font: inherit;
}
