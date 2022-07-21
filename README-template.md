# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)


## Overview

 Product preview card component UI design to code(HTML,CSS) 

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.jpg)


### Links

- Solution URL: [solution URL](https://github.com/purna-dev/Product-preview-card-component)
- Live Site URL: [live site URL](https://purna-dev.github.io/Product-preview-card-component/)

## My process
First i code for desktop device then code for mobile device

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned

```html
<div class="container con_mob">

      <div class="product_item pro_mob">
        <div class="img_s">
          <img src="images/image-product-desktop.jpg" alt="Perfume image">

        </div>
         <div class="img_m">
          <img src="images/image-product-mobile.jpg" alt="Perfume image">
          
        </div>
        <div class="text_s">

          <h1>Perfume</h1>

          <h2>
            Gabrielle Essence Eau De Parfum
          </h2>

          <p>
            A floral, solar and voluptuous interpretation composed by Olivier Polge,
            Perfumer-Creator for the House of CHANEL.
          </p>

          <div class="price">
            <p>$149.99</p>
            <span>$169.99</span>
          </div>

          <div class="btn_cart">
            <button>  
              <div class="icon_cart">
              
              <img src="images/icon-cart.svg" alt="cart icon" > 

              </div>
              <p> Add to Cart</p></button>
          </div>

        </div>
      </div>

    </div>

```
```css
@media (max-width:800px) {
    .container{
        display: none;
    }
    .con_mob{
        max-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    }
    .pro_mob{
        flex-direction: column;
        max-height: 700px;
        width: 380px;
        align-items: center;
    }
    .img_s{
        display: none;
    }
    .img_m{
        display: block;
    }
    .img_m img{
        border-radius: 0.7rem 0.7rem 0 0;
            max-width: 380px;
            height: 300px;
    object-fit: cover;
    }

    .text_s {
    padding: 1rem;
    width: 350px;
}

.text_s h1 {
    font-family: var(--font-montserrat);
    font-weight: 300;
    letter-spacing: 0.3rem;
    text-transform: uppercase;
    font-size: 0.9rem;
    color: var(--Dark-grayish-blue);

}


    .text_s h2 {
    font-family: var(--font-fraunces);
    margin: 1rem 0;
    font-size: 2rem;
    line-height: 1.9rem;
    color: var(--Very-dark-blue);
    max-width: 300px;
}
.text_s p {
    font-family: var(--font-montserrat);
    font-size: 1rem;
    line-height: 1.4rem;
    max-width: 310px;
    color: var(--Dark-grayish-blue);
}

.text_s .btn_cart button {
    width: 320px;
}
.text_s .price p{
    font-size: 2.2rem;
}
.text_s .price span{
    font-size: 1rem;
}
}

@media (max-width:380px) {
    .pro_mob{
        max-width: 350px;
        margin: 1rem;
    }
    .img_m img{
        max-width: 350px;
    }
}
```



### Continued development

Grid
Flexbox
Mobile first workflow


### Useful resources

- [resource 1](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This helped me for align elements or items in right position. I really liked this pattern and will use it going forward.



## Author

- Website - [Purna](https://purnachandra.me/)
- Frontend Mentor - [@purna-dev](https://www.frontendmentor.io/profile/purna-dev)
- Linkedin - [@impurna](https://www.linkedin.com/in/impurna/)



