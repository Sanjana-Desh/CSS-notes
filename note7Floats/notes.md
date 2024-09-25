# Float
- float:left; 
-  When you apply the float: left; CSS property to the .left class, it makes any element with that class float to the left side of its containing element. 
- To align a single para to left we have:
* {
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

.block {
    width: 30vw;
    height: 30vw;
    background-color: #000;
    color: white;
    padding: 1rem;
}

.left {
    float: left;
}

.left-align {
    text-align: left; /* This will left-align the specific paragraph */
}

p {
    text-align: center; /* Default behavior for other paragraphs */
}

-  p{ 
    margin-left: 1rem;
    will not change the attacment to block
} 