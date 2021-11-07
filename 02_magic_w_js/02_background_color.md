To do some simple magic with `JavaScript` to change the background color based on what the user chooses 😉.

To do so, we will only be introducing something called `querySelector()`. As what we did before, we will take the value the user entered. Let's step up some steps: 

1. Give our body an id, so we can help `JavaScript` identify what background to change.

   ![img](https://lh4.googleusercontent.com/1qjO3GvgXg6Fup5FdM1pOpbDDHks1Bs0FfvHYsuzl64cxifeXSTHRntOUURhfaplZyHyCq6olVjn5lSE0Fpb5FW2DMPiFFFITLKGFDOMxm1LTtNHO_rpUjh8MU4RQpthZVKMSLl8)

2. Tell the user to `Enter a color`

   ```javascript
   let userColor = prompt("Enter a color")    console.log(userColor)
   ```

   ![img](https://lh4.googleusercontent.com/VwUL-kC88f277P3FVYdJYGYM3oF82WLvlmMr1tMDtNLjDuCi7el0XEFy0EEYFmWHzWBCjvcxx05wz62-vCMLd90zBygLcnYp5VmsNwZRZv2_woEyJT67xjAfLbh_6fPselaLyPsY)

   **Note 📝:**

   > Notice how we changed the variable name to make more sense 😇

3. Use `querySelector()`

   ![img](https://lh6.googleusercontent.com/PlsAHCJR4lNIK1JfQVpn1gKrkEcz46Qf9Mcw2L3zv__0o0dOaZ2G2dSth_CszAKIyqzDj2pzBJDYQZymjf5gmBQjDtPIkUvOCrqS2ZoYAy8ugl5Bxu6YBMJtt8jOGGZUtESlr8rb)

   **Note 📝:**

   > Remember for `id` we use `#` and for `classes` we use `.` before their names.

![img](https://lh5.googleusercontent.com/jqYsESWlJxpjmK4p-On4ag_SE4qOBWynwRchJUZQP7_Miw1vp8gC5fG6QkjTppSfNjR6B-ynPCJTwd4Yzq-bPZoEoGwxENM4yokcEsVlJauRKZivIgcV9svsZojJgfObWq7VGkZG)

4. Now to change something in the style of that element, we must put `.style`


![img](https://lh6.googleusercontent.com/zgl-m--d-ubyyorqK_dhYsUh5Q3uuqKaXaV2dLjoHIkWqmgfN3J3F7FU1JLX-xFsrlLWlvku9wAakMRMZQZbn9TGwsl9PrzUL1zLgIk1IcEWW9FQ1RKFUPBN-JVuCeMAgp6Qb1Rq)

After identifying the element and that we want to style it, 

5. We will say `.background`

![img](https://lh4.googleusercontent.com/qhmg_Dl4yKKpY9c-QsPKzs6abi6VKcm4m4SA-eQCew_whgqIEX76GraqXy3g3DbuqVU5uZysCrBfcLuHUihZUSbX3A-8nvjtfaxuY7wnfiMoWYvP3zaoCQoi7XVlc0weUhdo2Frz)

To test it out we can say:

```javascript
querySelector("#body").style.background = “red”
```

**Testing:** 

![img](https://lh5.googleusercontent.com/2d0pY_shp5L_ZntOAINrbdAud_bUjmrz3AOp8yOBmh5ggCe8KpeYzNJzNlKrjgk-LfigKBlHuDwCEgu8cZmXGLFEsm7iEt5RjFXchg7w3jkzfgjJxCuDrG9oC97xkEyBzN5nMCra)

**We got an Error! 😱**


![img](https://lh3.googleusercontent.com/kAkgorkzuGnujBeBVFaavaSVoXhtWPYA_495t-OqnLJLiDBaGVYytCGKDEM3i98KrnmNavnjv4zZy9Y7gcFZ5eVEaSIdXNgBQMZqgR5NoBtJwUXBFZKM0X_ooEK9_XIJL9zji9g2)

It says that it does not identify our `querySelector` that is on line 12 in the `index.html` page

**Fix ⚠:**

> We forgot to introduce something else that must be written before the `querySelector` which is `document`because `HTML` is a document when it gets loaded to the screen.

**Implementation:** 


![img](https://lh5.googleusercontent.com/3dFz6WeSh17t6n8KP8EYx2H8u2RcJGE6PFs8ZrsoVybPpeQNQZgxc6nnuXojH7SWVanIPWn9itnx6I4xmKae-sglYBRsACbhqEuoSEyVbGi-zkTRXYTuEKwF2KeHJujpUxwUa0mm)

AMAZING 😍

6. One thing left!! Which is replacing the `red` with the `userColor` rather than a fixed color 🔥


![img](https://lh6.googleusercontent.com/DyTMSqAlFAdWumPWvPgZ_52A6bodUaAguY0kabHD596NkVygc6kOpXwwCREBfNxAyQPtuRg85QtwOiMasBERf7gQ5U0hg9hgyl5WoFgVijaf7qU5oUvl6URCyzm35ZqFUuUcvCbY)

   

````javascript
let userColor = prompt("Enter a color")
console.log(userColor)
document.querySelector("#body").style.backgroundColor = userColor
````

This is some of `JavaScript` magic 🔥 `proud of you 👏🏻`

> Try testing `hex colors`, and do not forget the `#` 😉

