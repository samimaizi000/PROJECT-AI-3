# AI-CSC4301-BustTheGhost

## Description
In this project, we used Unity to implement/reproduce  "Bust the Ghost" game. <br />
* Create a 8x 20 grid <br />
* Have the ghost be placed in one of the cells according to a prior distribution of Ghost over location P(Ghost). <br />
    * Use a uniform distribution to start with. <br />
* when clicking  a cell, the player gets a color red/green/orange/yellow depending on how the far is the ghost is from the clicked cell. <br />

- [x] On the ghost: red <br />
- [x] 1 or 2 cells away: orange <br /> 
- [x] 3 or 4 cells away: yellow <br />
- [x] 5+ cells away: green <br />

* For this, define and use a **conditional probability distribution** P(Colour/Distance from Ghost). <br />
    * Use this probability to decide on the color to display. <br />
* After each click "t", the  **Posterior Probability** of the Ghost P(Ghost/ Colour) should be _updated_ and _displayed_ on the cells using **Bayesian inference**: <br />
    * P(Ghost_t)=P(Ghost/Color_t)=P(Ghost_t-1)*P(Colour/Distance from Ghost). <br />
    * P(Ghost_0)= P(Ghost/Color_0)= P(Ghost) the prior probability. <br />

* Do not forget to Normalize! <br />
* User can decide to "bust" a cell if ghost is in the cell; the player wins otherwise he/she looses. <br />


## Youtube Video
Demo on Youtube: https://youtu.be/3sb4wh_SJww <br />
