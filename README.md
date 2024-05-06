# CSSttR-assignment

## Week 1 - My Plan

### Assignment

I want to create a control panel. I have the following ideas:

- Retro Arcade Console: A screen with a joystick and buttons. Control the game.
- Smart Home Hub: The inside of a house and a control panel. Control lights, thermostat, etc.

### Inspiration

![Best-places-for-arcade-game-lovers-646417004](https://github.com/mtdvlpr/CSSttR-assignment/assets/46671786/78ded364-466a-447f-ab9d-083d119c5b5c)

![smart-home-800-4288469625](https://github.com/mtdvlpr/CSSttR-assignment/assets/46671786/41f24de0-81ba-40d7-b852-47e8952f5192)

### CSS Techniques

I want to at least use the following CSS techniques:

- CSS nesting
- style queries

### Challenges

CSS in general is a challenge for me. Especially creating something visually appealing.

## Week 2 - Design

I have decided to go with the Retro Arcade Console, because I think it will be more fun and also challenging.

I started with just a box with a square that can be controlled with a d-pad.

## Week 3 - Development

I created the arcade console around the screen and made the player a pacman, but I had some trouble getting the 3D effects right.

![first](https://github.com/mtdvlpr/CSSttR-assignment/assets/46671786/8e564bb5-d49b-4eaa-b053-86b677e5648a)

The rest of the week, I was unable to work on the assignment, due to personal circumstances, so I've got some work to do.

## Week 4 - Final work

I made the buttons in arcade style and got the 3D working.

![second](https://github.com/mtdvlpr/CSSttR-assignment/assets/46671786/ea789e9b-c870-4064-930b-1abe7764c104)

### Start of the week

I tried to add walls using `@container style` queries, but I couldn't get it to work, because it could only target the `--x` and `--y` min/max values and not the intermediate values. I tried setting the `--x` and `--y` values at the root and multiply them with 1000, set other, set bigger values that would be easier to calculate the step for, but nothing worked.  I used the following code to test the functionality:

```css
@container style(--x: xxx) {
  :root {
    body {
      background-image: linear-gradient(green, lightgreen);
    }
  }
}
```

I tried to make it more in line with the actual game by having the pacman move indefinitely, using anchor links, but I couldn't get it to work, because the previous animation would reset when the link was clicked, which caused the pacman to move in a weird diagonal way.

### End of the week

I did not manage to add walls, but I did add eatable dots that dissapear when the pacman eats them. I also managed to make the pacman move indefinitely, but I had to use radio buttons instead of links. I also added a winner text when all the dots are eaten.

## Reflection

I learned a lot about CSS, especially about container style queries and animations. I also used CSS nesting for the first time. I've used nesting in SASS before, but never in pure CSS. I think it's very nice that this feature was added in CSS. I am happy with the result, but I would have liked to add walls and ghosts as well.

## Retake

For the retake I have added an animation for the dots Pacman eats. They act like gelatine. I also added animated ghosts that move across the screen and I've used the CSS level 4 `oklch` color space.

![Screenshot 2024-05-06 102230](https://github.com/mtdvlpr/CSSttR-assignment/assets/46671786/dc3bed6c-c440-46dc-afdb-b26ddfb5510d)

