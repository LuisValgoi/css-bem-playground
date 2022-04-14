# VIDEO

- [https://www.youtube.com/watch?v=u-XKw585KqY&ab_channel=dcode](https://www.youtube.com/watch?v=u-XKw585KqY&ab_channel=dcode)

# WHAT IS

- CSS Naming Convention

# BLOCK

- Represents a whole component/structure

# ELEMENT

- Represents an element or a part of a `block`
- We only consider an element if it depends on the `block`
- *"Does it make sense to turn this element into a separated one?"*
    - If yes... then this will turn into a `block`
    - If no... then this is a `element`

# MODIFIER

- The minimal variants of a block.
- Example: Primary, Dark, Light....

# NOTE

- **YOU SHOULD ALWAYS** use the `__` to separate each part of the convention.
- **YOU SHOULD ALWAYS** preceded the previously part of the convention to the next one.
- **DO NOT** represent the HTML semantic into your classes.
- **DO NOT** represent the HTML hierarchy into your classes.

```jsx
<div class="user">
	<a class="user__anchor">
		Link
		<span class="user__anchor__icon">ICON</span>
	</a>
</div>
```

# EXAMPLE

```jsx
<div class="user">
	<img class="user__photo"/>
	<button class="button">
		Normal button
	</button>
	<button class="button button--state-success">
		Success button
	</button>
	<button class="button button--state-danger">
		Danger button
	</button>
</div>
```