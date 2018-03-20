# DOM Ironhack Cart @TODO

## Link:
  - https://github.com/ironhack-labs/lab-dom-ironhack-cart

## Purpose:
  - Learn how to select DOM elements and manipulate them
## What they do in the exercise:
  - I1: create a product in the cart
        and create a button that calculates total prize
  - I2: create another product
  - I3: calculate the total prize of the cart
  - I4: deleting the products
  - I5: create a field to add new products
## Issues:
  - as creating new products is a feature it should be done before;
    so that we avoid creating products by copypasting code in I2
    we keep the same logics as when we do the CRUD in the projects
  - If the exercise gives the student this snippet plus all the function names, it becomes a fill the gap:
  ```
    window.onload = function(){
      var calculatePriceButton = document.getElementById('calc-prices-button');
      var createItemButton = document.getElementById('new-item-create');
      var deleteButtons = document.getElementsByClassName('btn-delete');

      calculatePriceButton.onclick = getTotalPrice;
      createItemButton.onclick = createNewItem;

      for(var i = 0; i<deleteButtons.length ; i++){
        deleteButtons[i].onclick = deleteItem;
      }
    };
  ```
  - in function deleteItem(e){}, e is not a self-explaining name.
## Purposal:

## Good practices:
  - names have to be self-explaining
  - a name shouldn't be a single letter
## Typos: