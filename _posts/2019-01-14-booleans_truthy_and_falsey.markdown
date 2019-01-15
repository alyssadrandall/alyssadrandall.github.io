---
layout: post
title:      "Booleans == Truthy & Falsey"
date:       2019-01-15 01:31:23 +0000
permalink:  booleans_truthy_and_falsey
---


In our assignments, we learned that booleans control the flow in our programs. It is incredibly helpful to have if, elsif, until, unless, case, and many other types of methods that determine the outcome the user experiences. 

It didn't dawn on me until reading a bit more on booleans in David A. Black's "The Well-Grounded Rubyist" that every object in ruby has a boolean value of true or false - and every expression in ruby returns an object. That means every line of code one reads or right is a boolean, whether we think about it or not. To top it off, true and false are objects as well. If they weren't, as Black states, "then a pure Boolean expression like

100 > 80 

would have no object to evaluate to. (And > is a method and therefore has to return an object.)"


Due to every state being true or false, true and false can be thought of as 'states'. This can be tested on a multitude of expressions. 
Here are my favorites of Black's examples:

if (def m, return false; end)
    puts "Method definition is true!"
else
    puts "Method definition is false!"
end

result: "Method definition is true!"

if 100 > 50 
    puts "100 is greater than 50!"
else 
    puts "100 is not greater than 50!"
end 

result: 100 is greater than 50!"

So even though you aren't just asking the language to evaluate def m, it evaluates that method definitions are true (as in, they exist and can operate within ruby), and even though we aren't outright asking if "100 > 50," its able to express to you that it's true. 

We don't really think about the boolean and logic flow when we're programming, but it's good to reflect on the nature of booleans to more deeply understand the logic process and how you're incorporating it into your work. Remembering where you started can help you be more efficient and be a master of your program, making it your best work yet.  
