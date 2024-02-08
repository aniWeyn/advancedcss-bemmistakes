# BEM Mistakes

Propose better solution according to BEM to following examples

### Example 1
    <header class="card card__header">
        <h2 class="card card__h2">Cars</h2>
        <h3 class="card card__h3">Fiat</h3>
        <h3 class="card card__h3">Opel</h3>
        <h3 class="card card__h3">Volvo</h3>
    </header>

### Example 2
    <button class="btn btn--primary button--disabled" name="favorite">
        <span>🚀 </span>
        <span> Add to basket </span>
    </button>

### Example 3
    .card--dog {
        background-color: pink;
    }
    
    .card--cat {
        background-color: yellow;
    }

### Example 4
    .Newcard {
      border: solid 1px rgb(255, 242, 0);
      border-width: 2rem;
      max-width: 260px;
      padding: 10px;
      }

### Example 5
    <p class="card__description__text">
        Lorem ipsum dolor...
    </p>

### Example 6
> [!TIP]
> What is a purpose of section? does it make sense to call it "card"?

> [!TIP]
> There are more mistakes to fix here :)

    <section class="card">
        <article class="card article__dog">
            <aside class="article__dog aside">
                <figure class="article__dog figure">
                    <img src="..." alt="Dummy Image" class="" />
                </figure>
             </aside>
         </article>
    </section>

### Example 7
    .button--styled--disabled{
        background-color: orange;
    }

### Example 8
    <article class="card cat--card">
      ...
    </article>

### Example 9
    <article class="card card--dog card--dog--type1">
      ...
    </article>

### Example 10
    .card {
        border: solid 1px #000;
        max-width: 360px;
        padding: 20px;
    }
  
    .card {
        background-color: white;
        margin-bottom: 20px;
        padding: 15px;
        display: block;
        align-items: center;
        justify-content: center;
    }

### Example 11
    .card--dog--type1 header{
        background-color: green;
    }

    .card--dog--type2 header{
        background-color: purple;
    }

    .card--dog--type3 header{
        background-color: orange;
    }

### Example 12
    <button class="btn btn--primary btn--disabled" name="favorite">
      <span>🚀 </span>
      <span> Add to basket </span>
    </button>

### Example 13
    <main class="main__flex-wrap">
        ...
    </main>
> [!TIP]
> Why is it not a good idea to specify type of flex applied to element in the name of class?

    
### Example 14
    <section class="dog--flex">
        ...
    </section>

### Example 15
    <footer class="card__options">
      <div class="card__options-buttons">
       ...
      </div>
    </footer>

### Example 16
    <header class="">
        <h2 class="card__dog--poster">Dog Poster</h2>
        <h3 class="">Dog poster - 50nok</h3>
    </header>

### Example 17
    <header class="card__header">
        <h2 class="card__title--cat">NEW! Cat Poster</h2>
        <h3 class="card__subtitle">Cat poster - 50nok</h3>
    </header>

### Example 18
    <section class="catbox">
        ...
    </section>

### Example 19
    <button class="card_basked_button styled disabled">
        <span class="card_basket_button_icon">&#128722;</span>
        <span class="card_basket_button_text">Basket</span>
    </button>

### Example 20
    <header class="main_header">
        <h1>BEM</h1>
        <button class="styled disabled wishlist">
            <span>🚀</span>
            <span>Wish list</span>
        </button>
    </header>
    </header>

    <main class="main">
        <section>
        <section>
    </main>

### Example 21
> [!TIP]
> Why it is not a good idea to style cards based on `nth-of-type(even)`

    .card:nth-of-type(even) .card_basked_button {
        ...
    }
