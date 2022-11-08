# Basic CSS and Cascade hierarchy
`CSS` stands for Cascading Style Sheets, and that first word cascading is incredibly important to understand — the way that the cascade behaves is key to understanding CSS.
`Cascade` and the closely-related concept of `Specificity` are mechanisms that control which rule applies when there is such a conflict. The rule that's styling your element may not be the one you expect, so you need to understand how these mechanisms work.
Also significant here is the concept of `inheritance`, which means that some CSS properties by default inherit values set on the current element's parent element and some don't. This can also cause some behavior that you might not expect.
# Cascade
`Stylesheets cascade` — at a very simple level, this means that the origin, the cascade layer, and the order of CSS rules matter. When two rules from the same cascade layer apply and both have equal specificity, the one that is defined last in the stylesheet is the one that will be used.
# Specificty
`Specificity` is the algorithm that the browser uses to decide which property value is applied to an element. If multiple style blocks have different selectors that configure the same property with different values and target the same element, specificity decides the property value that gets applied to the element. Specificity is basically a measure of how specific a selector's selection will be:
- An element selector is less specific; it will select all elements of that type that appear on a page, so it has less weight.
- A class selector is more specific; it will select only the elements on a page that have a specific class attribute value, so it has more weight.
`CSS selectors` follow a consistent hierarchy when it comes to specificity, so you can always tell which selector is the most specific. For example:
- Elements: If your selector is an HTML element, like p, it's not very specific. It applies broadly to every <p> element on the page.

- Classes: If your selector is a class, like .special Paragraphs, it's more specific. It could apply to more than one element, but only the ones where you've added that particular class.

- Ids: If your selector is an id, like #uniqueParagraph, it's very specific. A webpage should only include any given id once, so it should always be pointing to just one HTML element.
# Inheritance
`Inheritance` also needs to be understood in this context — some CSS property values set on parent elements are inherited by their child elements, and some aren't. While cascading and specificity are explicitly about resolving conflicts, inheritance is more about keeping your CSS orderly and avoiding unnecessary repetition. In other words, understanding inheritance will help you avoid conflicts in the first place.
# Non-inheritance
While many CSS declarations are passed down from parent to child, not all of them are. Properties like width, margin, padding, height and border are not inherited properties.
# Understanding how the concepts work together
These three concepts (cascade, specificity, and inheritance) together control which CSS applies to what element.
# controlling inheritance
CSS provides five special universal property values for controlling inheritance. Every CSS property accepts these values.
- inherit
Sets the property value applied to a selected element to be the same as that of its parent element. Effectively, this "turns on inheritance".
- initial
Sets the property value applied to a selected element to the initial value of that property.
- revert
Resets the property value applied to a selected element to the browser's default styling rather than the defaults applied to that property. This value acts like unset in many cases.
- revert-layer
Resets the property value applied to a selected element to the value established in a previous cascade layer.
- unset
Resets the property to its natural value, which means that if the property is naturally inherited it acts like inherit, otherwise it acts like initial.










