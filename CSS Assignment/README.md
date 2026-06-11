# Css-Assignment
# Exercise 1: Q1;The paragraph is red because #main-text is an ID selector, which has higher specificity than both the class (.highlight) and element (p) selectors. ID always wins in a normal specificity battle. Q2;When you chain selectors together (no space between them), their scores add up. #main-text.highlight combines an ID and a class, giving it a higher score than #main-text alone, so green wins. Q3; Same idea chaining an element and a class together scores higher than a class selector alone. The existing .highlight { color: orange } rule loses and green wins.

# Exercise2: Refer to Exercise2 folder, Q3:The > means direct children only. Both lists in the HTML have their <li> items sitting directly inside them, so all items correctly get bold. The difference would only matter if there were nested lists, > would skip them, while a regular descendant selector would bold everything. In this HTML there are no nested lists, so both approaches work, but > is the safer and more precise choice.

# Exercise3: Q4: p:nth-child(1) doesn't just look for the first <p> — it looks for an element that is both a <p> and the 1st child of its parent at the same time. In this HTML, the first paragraph happens to be the 1st child of .container so it actually works — but it's unreliable. If anything like a heading or div was placed before it, the first <p> would no longer be the 1st child and the selector would match nothing. A safer option is p:first-of-type, which simply finds the first <p> regardless of its position among its siblings.

# Exercise4: Refer to Exercise4 folder

# Exercise 5: SCENARIO A; The universal selector * targets every element on the page directly, including the <p>. The div rule sets the <div> to blue, and the <p> could inherit that blue from its parent — but inheritance only kicks in when no rule directly targets the element. Since * already targets the <p> directly with orange, inheritance never gets a chance. A direct rule always wins over an inherited value, even when that rule comes from the lowest-specificity selector possible. SCENARIO B;The text is green. Both rules target the <p> directly, so this is a pure specificity battle. The universal selector * has a specificity score of zero — it was designed to set broad defaults that any real selector can override. The class selector .highlight scores higher, so green wins. This demonstrates that even though * applies to everything, it sits at the very bottom of the specificity ranking and will always lose to a class, ID, or even a plain element selector.

# Exercise 6: Refer to folder Exercise6


