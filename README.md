# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](.assets/images/screenshot.jpg)

### Links

- Solution URL: [solution here](https://your-solution-url.com)
- Live Site URL: [live site here](https://grid-testimonials-e2416c.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I understood better and Learned to use the grid,especially the grid-column, grid-row and grid-template-columns properties with media-queries, which give the desired effects on the project. 

In addition, I tried to use the :root selector to arrange the project colors, and the flexbox to position the profile photos with their respective names and
subtitles.

As we can see in the excerpts below:

```html

  <article class="card_one">
      <div class="image">
        <div>
          <img src="assets/images/image-daniel.jpg" alt="Daniel" class="avatar">
        </div> 
        <div>
          <h4 class="name_one">Daniel Clifford</h4>
          <h5 class="subtitle">Verified Graduate</h5>
        </div> 
          <img src="assets/images/bg-pattern-quotation.svg" alt="" class="quotes">
      </div>
      
      <h1>
        I received a job offer mid-course, and the subjects I learned were current, if not more so, in the company I joined. I honestly feel I got every penny’s worth.
      </h1>
               
      <p>
        “ I was an EMT for many years before I joined the bootcamp. I’ve      been  looking to make a transition and have heard some people who had a
        amazing experience here. I signed up for the free intro course and found it incredibly fun! I enrolled shortly thereafter. The next 12 weeks was the best - and most grueling - time of my life. Since completing the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”
      </p>
    </article>

    <article class="card_three">
      <div class="image">
        <div>
          <img src="assets/images/image-kira.jpg" alt="Kira" class="avatar">
        </div> 
        <div>
          <h4 class="name_three">Kira Whittle</h4>
          <h5 class="subtitle_white">Verified Graduate</h5>  
        </div>
      </div>
         
      <h1>Such a life-changing experience. Highly recommended!</h1>
   
      <p>
        “Before joining the bootcamp, I’ve never written a line of code. I    needed some structure from professionals who can help me learn programming step by step. I was encouraged to enroll by a former 
        student of theirs who can only say wonderful things about the program. The entire curriculum and staff did not disappoint. They were very hands-on and I never had to wait long for assistance. The agile team 
        project, in particular, was outstanding. It took my learning to the next level in a way that no tutorial could ever have. In fact, I’ve often referred to it during interviews as an example of my developent
        experience. It certainly helped me land a job as a full-stack developer after receiving multiple offers. 
        100% recommend!”
      </p>
    </article>
    
    <article class="card_five">
      <div class="image">
        <div>
          <img src="assets/images/image-patrick.jpg" alt="Patrick" class="avatar">
        </div>
        <div>
          <h4 class="name_five">Patrick Abrams</h4>
          <h5 class="subtitle">Verified Graduate</h5>
        </div>
      </div>
           
      <h1>
        Awesome teaching support from TAs who did the bootcamp themselves. Getting guidance from them and learning from their experiences was easy.
      </h1>

      <p>
        “ The staff seem genuinely concerned about my progress which I find really refreshing. The program gave me the confidence necessary to be able to go out in the world and present myself as a capable junior developer. The standard is above the rest. You will get the personal attention you need from an incredible community of smart and amazing people.”
      </p>
    </article>   
```

```css

.cards {
  display: grid;
  grid-template-columns: 1fr;
  gap: 20px;
  margin: 20px;
}

.cards .image {
  display: flex;
  align-items: center;
}


@media(min-width: 640px) {
  .cards {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media(min-width: 1280px) {
  .cards {
    grid-template-columns: repeat(4, 1fr);
  }

  .card_one {
    grid-column: 1/3;
  }

  .card_five {
    grid-column: 2/4;
  }

  .card_three {
    grid-column: 4;
    grid-row: 1/4;
  }
}
```
### Continued development

With this project, I realized that I have to improve my skills in responsiveness, flex and grid and refine them so that I can use them in the future in personal projects and thus advance in web development so that I can take the next step in my career. In the future, I intend to learn to use frameworks like Bootstrap, preprocessors like SASS and other languages ​​like REACT JS, for example.


### Useful resources

- [Grid and Flexbox usage](https://www.youtube.com/watch?v=RCBdm4YTVpQ) - This helped me to position the cards as proposed in the project, as if they were pieces of a puzzle. Also, it helped me to flex position the divs with the profile picture next to their name and subtitle respectively.

- [:root usage](https://tipscode.com.br/variaveis-css-um-guia-basico-de-como-criar) - This is an amazing article that helped me to finally understand the use of Variables in CSS. I recommend to anyone who is still this concept.


## Author

- Github - [Ruan Silva Gaspar](https://github.com/RSG27)
- Frontend Mentor - [@RSG27](https://www.frontendmentor.io/profile/RSG27)
- Linkedin - [My Linkedin](https://www.linkedin.com/in/ruan-silva-gaspar-a13a89226/)

## Acknowledgments

Here I leave my thanks to the youtube channel tbsankara and the tipscode site for helping me in the solution of this project.
