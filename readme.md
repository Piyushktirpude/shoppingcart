# React Redux Project : Shopping Cart App

- ## [Project Live Link](https://shopping-cart-app-codehelp.netlify.app/)

> ### Social Media Links:

- ### [Portfolio Website Link](https://www.findcoder.io/u/atulsinghatul)
- ### [Linkedin Link](https://www.linkedin.com/in/atul-singh-082529249/)
- ### [Youtube Link](https://www.youtube.com/channel/UCBNc9Vs9mAFxnAKjzWRqDFQ)
- ### [Hashnode Link](https://atulsinghatul.hashnode.dev/)

## Name : Atul Singh

---

**The project took almost 5hrs to complete.**

**What I learned in this project :**

> **_How to Create Redux_**

- _**1:** createSlice()_

```
import { createSlice } from "@reduxjs/toolkit";

export const CartSlice = createSlice({
 name: "cart",
 initialState: [],
 reducers: {
   add: (state, action) => {
     state.push(action.payload);
   },
   remove: (state, action) => {
     return state?.filter((item) => item.id !== action.payload);
   },
 },
});

export const { add, remove } = CartSlice.actions;
export default CartSlice.reducer;
```

- _**2:** Global centralised Store_

```
import { configureStore } from "@reduxjs/toolkit";
import { CartSlice } from "./Slices/CartSlice";

export const store = configureStore({
  reducer: {
    cart: CartSlice.reducer,
  },
});
```

- _learn useSelector() hook_

- _learn useDispatch() hook_

- _How link Slice Component to Global Store_

- _How link Redux to React using Provider_

---

![Project Screenshot](https://img.shields.io/badge/ShoppingCartApp--ReactReduxProject-blue)
![shopping-cart-home-page](https://user-images.githubusercontent.com/112545072/230768808-59d32d33-5416-4d19-8a98-8817d3f1200a.png)

![shopping-cart-page](https://user-images.githubusercontent.com/112545072/230768819-f9ddce11-ccbd-443e-af80-241e3714e57f.png)






