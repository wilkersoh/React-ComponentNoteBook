# React-ComponentNoteBook

### Toggle Check box

```javascript
const onCheckboxChange = (cartID) => {
  setCartItem((prev) => {
    const updated = prev.map((cart) => {
      return cart.id === cartID
        ? { ...cart, isChecked: !cart.isChecked }
        : cart;
    });
    return updated;
  });
};
```
