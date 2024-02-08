# BEM in practice

## Part 1 - BEM
Below you can see examples of code and style from class exercises: 
- *Week 4 - Exercise 01 - Applying BEM and styling*
- *Week 5 - Exercise 01 - Inheritance and BEM* 

**Discuss** in groups of two below examples and **propose better solution** according to BEM principles if needed. 

If you need help feel free to use [BEM Naming Cheat Sheet](https://bem-cheat-sheet.9elements.com/) or discuss it on MS Teams -> Team: AdvancedCSS 2024 -> Channel: [General](https://teams.microsoft.com/l/channel/19%3AGcJsLef6WAE6qb-9gr01mLK-AJ8W7tCQaUsF15g5AJs1%40thread.tacv2/General?groupId=05ca134d-fae1-48db-b017-a4769681310d&tenantId=09a10672-822f-4467-a5ba-5bb375967c05)

## Part 2 - GitHub Collaboration
In addition to the above BEM exercise, in your group, practice Git collaboration:

1. Clone this repository to your machine.
2. One student takes exercises with even numbers, and the other student takes exercises with odd numbers.
3. Practice creating branches, pull requests, and merging.
4. Create a branch for each example.
5. Add your solution.
6. Create a Pull Request for that change.
7. Your colleague needs to approve your Pull Request.
8. Merge your changes into the "main" branch.
9. Repeat steps 4-8.
10. **Do not delete the Feedback branch.**

## Example 1
    <header class="card card__header">
        <h2 class="card card__h2">Cars</h2>
        <h3 class="card card__h3">Fiat</h3>
        <h3 class="card card__h3">Opel</h3>
        <h3 class="card card__h3">Volvo</h3>
    </header>

#### Solution 1:
    <header class="card__header">
        <h2 class="card__header--title">Cars</h2>
        <h3 class="card__header--subtitle">Fiat</h3>
        <h3 class="card__header--subtitle">Opel</h3>
        <h3 class="card__header--subtitle">Volvo</h3>
    </header>
> [!NOTE]
> block: card, element: header, modifier: title/subtitle

#### Solution 2:
    <header class="card__header">
        <h2 class="card__header card__header--title">Cars</h2>
        <h3 class="card__header card__header--subtitle">Fiat</h3>
        <h3 class="card__header card__header--subtitle">Opel</h3>
        <h3 class="card__header card__header--subtitle">Volvo</h3>
    </header>
> [!NOTE]
> this solution can be correct in case class `card_header` consist of some styles that cannot be inherit and needed to be specified and are shared between all headers

## Example 2
    .card--dog {
        background-color: pink;
    }
    
    .card--cat {
        background-color: yellow;
    }

## Example 3
    .Newcard {
      border: solid 1px rgb(255, 242, 0);
      border-width: 2rem;
      max-width: 260px;
      padding: 10px;
      }

## Example 4
    <p class="card__description__text">
        Lorem ipsum dolor...
    </p>

## Example 5
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

## Example 6
    .button--styled--disabled{
        background-color: orange;
    }

## Example 7
    <article class="card cat--card">
      ...
    </article>

## Example 8
    <article class="card card--dog card--dog--type1">
      ...
    </article>

## Example 9
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

## Example 10
    .card--dog--type1 header{
        background-color: green;
    }

    .card--dog--type2 header{
        background-color: purple;
    }

    .card--dog--type3 header{
        background-color: orange;
    }

## Example 11
    <main class="main__flex-wrap">
        ...
    </main>
> [!TIP]
> Why is it not a good idea to specify type of flex applied to element in the name of class?

    
## Example 12
    <section class="dog--flex">
        ...
    </section>

## Example 13
    <footer class="card__options">
      <div class="card__options-buttons">
       ...
      </div>
    </footer>

## Example 14
    <header class="">
        <h2 class="card__dog--poster">Dog Poster</h2>
        <h3 class="">Dog poster - 50nok</h3>
    </header>

## Example 15
    <header class="card__header">
        <h2 class="card__title--cat">NEW! Cat Poster</h2>
        <h3 class="card__subtitle">Cat poster - 50nok</h3>
    </header>

## Example 16
    <section class="catbox">
        ...
    </section>

## Example 17
    <button class="card_basked_button styled disabled">
        <span class="card_basket_button_icon">&#128722;</span>
        <span class="card_basket_button_text">Basket</span>
    </button>

## Example 18
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

## Example 19
> [!TIP]
> Why it is not a good idea to style cards based on `nth-of-type(even)` in context of shopping cards?
> In which context it will be a good idea?

    .card:nth-of-type(even) .card_basked_button {
        ...
    }

## Example 20
> [!TIP]
> Why it is not a good idea to create repetitive styles based on id?
> In which context we should use ids?

    #wishlist {
        ...
    }

## Example 21
    <main class="main_flex-container">
        ...
    </main>

## Example 22
> [!TIP]
> BEM stands for block__element--modifier, is "cat" and "dog" an element? 

    <section class="card-section__cats">
        ...
    </section>

## Example 23
> [!TIP]
> Let's assume that in some case it make sense to call a section "cat" or "dog", the section "cat" will consist of multiple cards of cats, and the section "dog" will consist of multiple cards of dogs. Let's not focuse here on BEM. Nevertheless, how could you improve on class naming?
> 

    <section class="cat">
        ...
    </section>

## Example 24
    .button__div1,
    .button__div2 {
        display: flex;
        flex-direction: row-reverse;
    }

## Example 25
![image](https://github.com/aniWeyn/advancedcss-bemmistakes/assets/23743322/57049158-a239-4853-aa76-c2cf63e443fe)

## Example 26
    header {
      background-color: hsl(180, 31%, 95%);
      ...
    }

    header>button {
      border: none;
      ...
    }

    header>button:hover {
       background-color: hsl(180, 25%, 73%);
    }

    header>button:active {
      background-color: hsl(180, 29%, 50%);
    }

## Example 27
In what scenarios is it advantageous to use a class name that represents the animal, and in what scenarios would it be preferable to use a generic name like 'product_01' or 'product_02'?
