---
layout: post
title:  "General Progress"
date:   2018-12-12 15:54:37 +0800
---

# General Progress


2019/02/19
* Find it difficult to ask questions about Gatsby JS. Could not find the right community for it.
* Keep switching between "start from ground up" and "continue making progress on existing project"
* Might have to find a temporary solution when it comes to the main page design.
    * Have not been able to move the blog section into index.js
    * Forgot to put any styling inside the index.js's `<Layout></Layout>` section
    * **remember to edit footer.js later**

2019/02/20
* Finish the HTML/CSS part of the 404 page. https://codepen.io/zhouxiang19910319/pen/GzeePV, how to convert this into a randdom quote machine AND put it into my gatsby blog is another question.

* Had some progress when it comes to the gatsby blog. Learned the difference between using bootstrap VS react-bootstrap in gatsby site.

2019/02/21
* Had some progress on re-doing the main page, eventually chose CSS in JS to do it.
* Finished index page's layout.

* W3 project had some progress too. Successfully get the weather data using open weather API + fetch method. 
* Next steps: 
  * Code the UI
  * Put in all the elements (icons + fonts + colors etc), find the right ones.

2019/02/22 W3 Progress
* Steps: 
1. about swapping out all the icons: maybe use font awesome? 


`<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.2/css/all.css" integrity="sha384-fnmOCqbTlWIlj8LyTjo7mOUStjsKC4pOpQbqyi7RrhN7udi9RwhKkMHpvLbHG9Sr" crossorigin="anonymous">
` 

2. **No need to differentiate day and night**
3. Use switch cases when it comes to the icon.
4. Code out the general UI?
5. Decided the main font of the project: Open Sans
6. Icon list:
    * Sun:  `<i class="far fa-sun"></i>`
    * Cloud: `<i class="fas fa-cloud"></i>`
    * Rain: `<i class="fas fa-cloud-showers-heavy"></i>`
    * Thunderstorm: `<i class="fas fa-bolt"></i>`
    * Snow: `<i class="fas fa-snowflake"></i>`
    * Mist: `<i class="fas fa-water"></i>`

7. Weather condition codes
    * 2xx: Thunderstorm
    * 3xx: Rain
    * 5xx: Rain
    * 6xx: Snow
    * 7xx: Mist
    * 800: Sun
    * 80x: Cloud

2019/02/24

# **Side project idea.**
# **Built a site that can generate charts based on numbers that user can key in. So that youtube Channels like hardware unboxed do not need to spend hours of time building charts.**


2019/03/03

* Keep making changes to the latest version of my portfolio.
* Came up with a new design idea when it comes to the mobile version of the site.
* Finished another version of my own portfolio. https://mattzhou.com/

2019/03/07
* ~~Page height is related to portfolio site displayed funny on small screen phone, like iphone 5.~~
* I need to make sure that however the page get zoomed in , all of the content on the page (text,pics) must fit in on the screen.
* **Done with my portfolio for now.** https://mattzhou.com

2019/03/08
# **Side project idea.**
# **Google Chrome / Firefox / Safari bookmark syncing tool**

* Successfully made slowpacedcoding blog posts sorted by date. 

```
export const pageQuery = graphql`
  query BlogIndexQuery{
      allMarkdownRemark
      (sort: { fields: [frontmatter___date], order: DESC })
      {
        edges{
          node{
            id
            frontmatter{
              path
              title
              date
              author
            }
          }
        }
      }
    }
`
export default blogPage
```

* Changed some of the styling on blog post page.
* Tasks left to do: 
    1. Make the slowpacedcoding icon a responsive image using : `gatsby-image`. ✅
    2. Find out why individual blog posts does NOT have any styling at all.

2019/03/09

* https://www.gatsbyjs.org/packages/gatsby-plugin-styled-components/

2019/03/10 (got a lot done today)

* Swapped out the logo with an png image.
* Centered the saying image using flexbox + margin: 0 auto. (had to use both of them).
* Solved the issue where the color you see in photoshop is not the same as the color you see on your web.

TODO LIST: 
1. Add in the footer.
2. Finish the random quote machine on the 404 page.
3. Move blog.js to the index page.
4. Fix the styling for the individual blog posts.


2019/03/15
# **Side project idea.**
# **Build a macOS finder clone using VUE/React JS.**