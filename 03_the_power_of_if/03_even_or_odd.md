Knowing that `JavaScript` can control styling elements, now we will learn how to add text to an element using `JavaScript`. As what the title is saying, we will check if the number the user will be entering is even or odd? And print on the screen `Your number is even` when it is `Even` and `Your number is odd` when it is `Odd`. Simple concept that will be fun 😉

1. Our layout will be:

   ```javascript
   <script>
     let number = prompt("Enter your number") if (// Condition){" "}
     {console.log("Your number is even")} else{" "}
     {console.log("Your number is odd")}
   </script>
   ```

2. Knowing the condition

   **❓ Question:**

   > How will we know if the number is even or odd?

   **🤓 Answer:**

   > We will use `%` modulus, we only mentioned it with the mathematical operations. IT IS TIME to know what modulus do?

**Note 📝:**

> Modulus helps with knowing the reminder of a division, so if we have 7 students and we want to know how many will be the reminder if we divided them by 3: `7 % 3`:

![img](https://lh4.googleusercontent.com/z9qGUMDgt3-oFyS6crVwR3NdqVaq8VifMj5Iq6n_y7bTVj29xKpdkAx3Ryn0Pyyt53nFP7tq1ZYhdgifv26UQf2fzq4oLV0TbOVI-xx0cBwRlp7ujvN9yXi0La_MOXKJVhtNctWF)

The result will be `1` notice how only one left. On the other hand the result from division is `2` because we only got two boxes.

**Note 📝:**

> Divisions and reminders will only give a whole number. In programing we do not get fraction numbers out of them unless we played around more with it ( I encourage you to look it up 😉)

**Implementation:**

In this our condition will be `number % 2`:

1. If `number` was even, then all will be distributed fairly and value will be `0`
2. If `number` was odd, then all will be distributed unfairly and value will be `1` because their will always be one left

![img](https://lh5.googleusercontent.com/6c37-Yqx-sxNHcCkUpKqAFL8fjF_EFvzV3QO8AVkixbbwbn3uHifasVWSRyTS6zuofAkfdfKKqm4zZ51WFKZm3yFPWsrFVI0MO9viQEg7jBpaekVgdKT5T2gO5N_D9muUPhmp5zp)

Weird!! When we enter something even it says odd and vise versa 🤔

**Fix ⚠:**

> As we said when `number % 2` is even the result must be zero and when the number is odd the result must be one.

The fix will be `if (number % 2 == 0)`

![img](https://lh5.googleusercontent.com/Njo0PdzyMwOpb728DO6MH6W4knvHE_6Xawx2DsH6DRAGTaGHzdX50hjsyMBqgTvrKItoB0YqBh2wfYItRqJKntoBChPOEWUr6GJqd9IqgkmZgFMakx6XH68zj2jRh_W1xqwPgdNj)

> Which means `if (number % 2 == 0) ` then your number is `even` and

**01_InnerHTML**

Are you tired of opening the `inspect` to see the `console` result? I know I do 👀Time to learn more amazing things 🔥

**❓ Question:**

> How did we change the screen background last time?

**🤓 Answer:**

> Using `document.querySelector()`, we will use it again but adding something new to this sentence

1. First let's give the `<body>` an `id` so we can use it

![img](https://lh4.googleusercontent.com/odICp2knqI9rfg5tBaStcwhBJPus5NLJgNQowpTrsR-5UMcUvKaEKFU10Sydu6tlc18hrJbs1bLsfpznQ-j0jsiQyxqs5XgGiuzLSNyYQRIG3ybgWw7LmJUhSImJVpPCmIO53cih)

2. Add ` document.querySelector()``to both statements calling that  `id`

   ![img](https://lh6.googleusercontent.com/JEKBSx563MF4LWR1KNbnmUg-ss2Ogih_NDqlH-2gOYFL3aKDU_ne0ivkIH3_lWPy4NfAAwi1rmK3lY1ya2lv81w1llTtO0Z7anOXtn5Sw73_ctbIx5lfi4S_jzTLW4G47A4pTdXr)

3. Now our additional command is `.innerHTML`

![img](https://lh3.googleusercontent.com/SEszFGuxhIUC5Jo09WW7CZv1XR5sDigmGOF7OYx3H4kmrKqbBU6RVMZX4Q2dYCL-3LWCDJcdcXWYbeRB4cUL6DGQEmt45A1qzKvZTKQKI5R_qWciE7AOxk31FujM56ypqOm6BfZL)

4. Adding out `innerHTML` to equal the sentence we want

![img](https://lh5.googleusercontent.com/l2DCENXZSO9r58k6WzDENDlVkI6xd4UHdnqLedOycijIzEREdzFqUpc9nRdv_hSv9_5IMHlBQyTzxXZOIaBJ8w68CHdgrJDUqBpJ3sp_20fu2NTcYnF7bRJYJBB_TrIYt3Z3a2y8)

5. Close the `inspect` we do not need it 😍 Let's try it!!!

![img](https://lh6.googleusercontent.com/S_06XM_9LPt3VMuqRQdE4WqOuAAJl8IuOkmHBnfOvsnSqZqtTmA-caHIskAR4jN_AGFdRFmsXmtA8QqS-tygHAxgoS05j4kGpFmCxx8zTxxf5jBBP1U01_v7zADw16OtgJ8gAeWN)

NICE 😍🔥 `proud of you 👏🏻`

**Note 📝:**

> What `innerHTML` does is add content inside the `HTML` that we choose which is the `#body`. So we can add `HTML` elements as well 🔥

**Implementation:**

![img](https://lh5.googleusercontent.com/Vm74deXaQ2nn_eaoPo-IyKeXG-e5bRuqZyKlqqKhBuMlgVSzeD63zgx3a9WaJyz7k0WeN8egc-DL64bDuft0UadaEG_KzFTcOIIqC2tRG6uPysi3D-59JaInhUlOVrBQ2d9KZCH-)

So it is not only `text` it can be any element we want 🔥

```javascript
<script>
  let number = prompt("Enter your number") if (number % 2 == 0){" "}
  {(document.querySelector("#body").innerHTML = "<h1>Your number is even</h1>")}{" "}
  else{" "}
  {(document.querySelector("#body").innerHTML = "<h1>Your number is odd</h1>")}
</script>
```

**02_Alert**

Now what if the user entered values we do not want, for example left it empty 🤔. What can we do?

As future programmers you must be prepared for everything! (or most things 😜)

**❓ Question:**

> Is there a name for when a variable is empty?

**🤓 Answer:**

> YES, it is called `null`, which is invaled argument and some languages like `JavaScript` when asked for a number and the value is `null` it gets replaced with a `zero`, That is why in the `Even or Odd` website when we leave the `input` empty it gave us `even`. `0` is an `even` number. `Mind Blown 🤯`

This means we need another `if statement` to see if `number == “”` where `””` are nothing so they are empty

![img](https://lh5.googleusercontent.com/i9ubedctYZ0ymysnkXD5gz_NMHMAd4qAhTEd7oZIkyD_CCZKJKiqL1nLSJwGTTkxSA7FyPazOyX9SuZJBInzkiiG-UlLj31TDz_wGrBh-yE55eZv9LgT1lrWeO7UZ_uAXdKKEOja)

One isse left, as programmers we have to keep our code clean and neat

**Fix ⚠:**

> Using something from the `if statement ` which is `else if`

**Implementation:**

![img](https://lh3.googleusercontent.com/2v6dTV9_AViatXs6BW3MO_29NOujaUdSuUR5QT6G6hjbwLiEmtVohr0yW8iJbAu37GQcygo1ShvSegdvO8KD1COPw82FVTcLRSWeve8QsqQNjFvLMzuKfwIEoztKLgXnGZb4du5B)

```javascript
<script>
  let number = prompt("Enter your number") if (number == ""){" "}
  {(document.querySelector("#body").innerHTML = "<h1>Your number is null</h1>")}
  else if (number % 2 == 0) {
    (document.querySelector("#body").innerHTML = "<h1>Your number is even</h1>")
  } else {(document.querySelector("#body").innerHTML = "<h1>Your number is odd</h1>")}
</script>
```

![img](https://lh4.googleusercontent.com/yFq6wtj-8P_fCjWbm1ZlnJ9Z-jncDRxZmqzeJdTz5_7Co47SiWcuLz1BLKVMuH7AN48ucIy3e9ueWO2NjUAW3UEGkkDBUqYYVZOVIlQpO9MDgbao2hqSjPTxI0-4s4Y2HprPyMco)

**Note 📝:**

> You can add as much `else if` as you need, BUT first must be `if` and last must be `else`

> Notice that `else if` has a condition like `if` and that `else` does not have it.
