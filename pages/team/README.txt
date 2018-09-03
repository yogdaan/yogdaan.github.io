Suppose two planes are hidden and are going to be shown 1 by 1 on hover container. E.g.On hover container, flips plane A (0.7s motion) after that flips plane B(0.3s motion), on mouse out container, transit reversely, i.e. flips plane B(0.3s motion) after that flips plan A(0.7s motion). 

We can do that by specifying `transition-delay` on `:hover` state. Yes.
E.g.  

    A:hover { transition-delay:0 }  /* A first */
    B:hover { transition-delay:0.7s }  /* 0.7s for A motion duration */

Then, on normal state (see it as mouse out state)

    A { transition-delay:0.3s }  /* 0.3s for B motion duration */
    B { transition-delay:0s }  /* B first */
