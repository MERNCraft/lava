# The Floor is Lava #

[Demo](https://MERNCraft.github.io/lava)

A simple CSS-only game using `:hover` and `z-index` to create a fail state. It was designed to showcase a way to restart a CSS game after the player has lost.

At the start of the game the CSS for the `.lava` element has no rule for `:hover`. When you press the Start button, a `:hover` rule is added that sets the `z-index` of the `.lava` element to `1`, bringing it in front of the Start button.

If your mouse remains over the Start button, you are safe. But the Start button starts to move and get smaller, so you must keep your mouse over it, or the `.lava` will come to the front and display both a "You Lost" message and a link that has been styled to look like a button.

The link simply reloads the page, so the checkbox input is restored to its original state.

It's fun (for about 10 seconds) on a computer with a mouse, but it won't be playable on a touchscreen, where there is no way to detect a `:hover` state.