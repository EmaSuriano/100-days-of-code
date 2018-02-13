# 100 Days Of Code - Log

### Day 1: January 24, Thursday

**Today's Progress**: First day of the challenge! Feeling really good :D Today I've working on the react-responsive-gallery adding new examples to the demo page and also see some improvements that I can do to get a better component. It looks pretty neat at this point, but my fear is that as CSS grid do not improve the compatibility with another browser the gallery won't have any success, but it's really fun to write libraries :D
Another very important point is, this library was originated by the CSS grid course by Wes Bos which is excellent! So kudos to him!

#### Overall status: Good

**Link(s) to work**

1. [React Responsive Gallery](https://github.com/EmaSuriano/responsive-react-gallery)
2. [Css-grid course](https://cssgrid.io/)

### Day 2: January 25, Thursday

**Today's Progress**: I continue working on the react gallery library, this time refactoring almost all the library to decouple the images from the modal. Now this one is being controlled by the gallery itself. Also, add the possibility to pass an onClick prop to the gallery, so if anyone wants to do something different from displaying the modal they can!

#### Overall status: Regular

**Link(s) to work**

1. [React Responsive Gallery](https://github.com/EmaSuriano/responsive-react-gallery)

### Day 3: January 26, Friday

**Today's Progress**: I started working on my portfolio (which has been abandoned for a while with a WIP message 😅). This time I decided to use Gatsby because I want to create a blog inside my portfolio, so I can start writing blogs there and in the future move them to medium. Also, if I made this log a bit richer in the information I can create one entry every day for the blog. So I use template for gatsby which has a beatiful UI and also the amount of pages that I want. So what do I add to the portofolio?

* Add at least one entry to the blog
* Change About page
* Change Contact page
* Use my free url and see how it goes.

#### Overall status: Good

**Link(s) to work**

1. [My Portfolio](https://github.com/EmaSuriano/emasuriano.github.io)
2. [Gatsby Starters](https://www.gatsbyjs.org/docs/gatsby-starters/)
3. [Lumen starter](https://github.com/alxshelepenok/gatsby-starter-lumen)

### Day 4: January 27, Saturday

**Today's Progress**: Today I've looking in more detail the gatsby starter and I finally understand how to enable comments inside the posts. It's using Disqus which is really great but for now I will disable it. My focus right now is to have a portfolio that can be send to another person, at least with my photo 😂 Also I tried to upload the portfolio to my DNS (emanuelsuriano.design) but I can't. In both platforms, there was a message saying that the changes may take up to 24 hours son lets hope that by tomorrow everything is gonna be fixed. I still need to continue working on the portfolio but it's looking good!

#### Overall status: Medium

**Link(s) to work**

1. [My Portfolio](https://github.com/EmaSuriano/portfolio-gatsby)
2. [My DNS](http://emanuelsuriano.design/)

## Day 5: January 28, Sunday

**Today's Progress**: I learned how to implement plugins inside gatsby, this time I wanted to use this one gatsby-remark-images. This plugin transform the img in mardown to beatiful lazy load images that have a blur effect while they are loading, so it's really cool because the content wont be start to gittering while are loading.

### Overall status: Medium

**Link(s) to work**

1. [My Portfolio](https://github.com/EmaSuriano/portfolio-gatsby)
2. [My DNS](http://emanuelsuriano.design/)
3. [Netlify link](http://emasuriano.netlify.com/)
4. [gatsby-remark-images](https://www.npmjs.com/package/gatsby-remark-images)

## Day 6: January 29, Monday

**Today's Progress**: I wrote my first serious article on my page, telling how I get my portfolio in one night. It took me a lot of work and time but I am really happy with the final product. I have a lot of grammatical mistakes but fortunately, my girlfriend helped me to solve them 😘

### Overall status: Good

**Link(s) to work**

1. [My Portfolio](https://github.com/EmaSuriano/portfolio-gatsby)
2. [Link to the Post](http://emasuriano.netlify.com/posts/how-i-made-my-page-in-1-night/)

## Day 7: January 29, Monday

**Today's Progress**: I learned how to implement twitter cards in order to preview a beatiful card after pasting the link inside a tweets, so this is very important because the tweets seems more relevant with that card. Also get some fixes inside the previous article and upload my image inside the page.

### Overall status: Medium

**Link(s) to work**

1. [My Portfolio](https://github.com/EmaSuriano/portfolio-gatsby)
2. [Link to the Post](http://emasuriano.netlify.com/posts/how-i-made-my-page-in-1-night/)
3. [Twitter docs](https://developer.twitter.com/en/docs/tweets/optimize-with-cards/overview/summary-card-with-large-image)

## Day 8: January 30, Tuesday

**Today's Progress**: Today I've working with hotkeys in react, trying a few libraries like react-keydown, react-hotkeys, mousetrap and much more. I end up using any of them, because of the problem that if i want to use the shortcut I need to first focus the parent element. So tomorrow I will continue looking for the one that helps me solve this fucking task.

### Overall status: Bad

**Link(s) to work**

1. [react-hotkeys-example](https://github.com/EmaSuriano/react-hotkeys-example)
2. [react-hotkeys](https://github.com/greena13/react-hotkeys)
3. [react-keydown](https://www.npmjs.com/package/react-keydown)

## Day 9: January 31, Wednesday

**Today's Progress**: I continue working on the hotkeys system for a react application. We were using react-hotkeys to catch the keys and call function after pressing the combination that we want. THe problem was that if we defined a hotkeuys componentn that wraps a small componennt in our app the shortcuts will only work if we are focusing that component (wont be globally usable). So we end up with a solution of wrapping the whole application with ONE HotKeys componentn so wherever we are focusing the shortcuts will work and then if a small component want to add a new shortcut to the application, it will get the context and call a functions subscribeHandler. Also when it will unmount, it has to call the unsubscribeHandler too.
We kind of create a hotkeys system where any component can add or remove shortcuts via context, and in my opinion it's really slick!

### Overall status: Good

**Link(s) to work**

1. [react-hotkeys-example](https://github.com/EmaSuriano/react-hotkeys-example)
2. [react-hotkeys](https://github.com/greena13/react-hotkeys)

## Day 10: February 1, Thursday

**Today's Progress**: After getting a functional hotkey system with react-hotkeys I was wondering how react-hotkets work and why I only can call hotkeys while focusing the component that has the hotkeys binded. So I check out Mousetrap and for my surprise the library binds shorcuts globally so the whole context fix is not required anymore. Therefore I rewrite the hotkeys system and it endup giving a better solution with less code (less code === easy and simple to read).

### Overall status: Good

**Link(s) to work**

1. [react-hotkeys-example](https://github.com/EmaSuriano/react-hotkeys-example)
2. [react-mousetrap](https://www.npmjs.com/package/react-mousetrap)

## Day 11: February 3, Saturday

**Today's Progress**: Another requirement was giving to us, we have to display a tooltip so the user will know which hotkey he has to press in order to call/focus/click any component of the application. Talking about the tooltip we didn't want to re invent the wheel so we use react-tippy which is a very simple and looking-good toltip! So we re-write the implementation and create a ShortcutWrapper which has very clean code and we think that it would be an excellent case for a new library! And that was what we did, we called it react-hotkey-tooltip. We've setup the repository, coverrals and travis CI using nwb create-library!

### Overall status: Good

**Link(s) to work**

1. [react-hotkey-tooltip](https://github.com/EmaSuriano/react-hotkey-tooltip)
2. [mousetrap](https://craig.is/killing/mice)
3. [react-tippy](https://github.com/tvkhoa/react-tippy)

## Day 12: February 4, Sunday

**Today's Progress**: Published react-hotkey-tooltip to npm v1.0.0 and improve README adding badges from shields.io

### Overall status: Regular

**Link(s) to work**

1. [react-hotkey-tooltip](https://github.com/EmaSuriano/react-hotkey-tooltip)
2. [shields.io](https://shields.io/)
3. [npm package](https://www.npmjs.com/package/react-hotkey-tooltip)

## Day 13: February 5, Monday

**Today's Progress**: Feeling like a dev-ops installing several tools: semantic-release, gh-pages, commitizen and tuning everthing with Travis CI. I'm having problems to release the package to npm, but it seems something on Travis conf.

### Overall status: Bad

**Link(s) to work**

1. [react-hotkey-tooltip](https://github.com/EmaSuriano/react-hotkey-tooltip)
2. [travis link](https://travis-ci.org/EmaSuriano/react-hotkey-tooltip)
3. [semantic-release](https://github.com/semantic-release/semantic-release)

## Day 14: February 6, Thursday

**Today's Progress**: Installing jest in react-hotkey-tooltip and starting to improve code coverage 💪 Let’s get 💯% coverage!
BTW: the library is on npm if anyone want to try it!

### Overall status: Regular

**Link(s) to work**

1. [react-hotkey-tooltip](https://github.com/EmaSuriano/react-hotkey-tooltip)
2. [travis link](https://travis-ci.org/EmaSuriano/react-hotkey-tooltip)
3. [npm package](https://www.npmjs.com/package/react-hotkey-tooltip)

## Day 15: February 7, Friday

**Today's Progress**: Achieving 100% coverage on react-hotkey-tooltip but now Travis is breaking while running the build process 😞 if I fix that, it will be time to create a beautiful home page for it 😍

### Overall status: Regular

**Link(s) to work**

1. [react-hotkey-tooltip](https://github.com/EmaSuriano/react-hotkey-tooltip)
2. [travis link](https://travis-ci.org/EmaSuriano/react-hotkey-tooltip)
3. [Coveralls](https://coveralls.io/github/EmaSuriano/react-hotkey-tooltip)

## Day 16: February 8, Saturday

**Today's Progress**: After trying several configurations for #TravisCI, I can say that it's working like a charm! 💪 There was a problem with semantic-release and the version of the package, so I wasn't able to upload it to npm due to an error, therefore coverrals coverage report was not being updated. Fortunalately, its working!

### Overall status: Good

**Link(s) to work**

1. [react-hotkey-tooltip](https://github.com/EmaSuriano/react-hotkey-tooltip)
2. [travis link](https://travis-ci.org/EmaSuriano/react-hotkey-tooltip)
3. [Coveralls](https://coveralls.io/github/EmaSuriano/react-hotkey-tooltip)

## Day 17: February 9, Sunday

**Today's Progress**: Deploying my webpage to GitHub pages using gh-pages from npm - zero configuration 😁 I'm considering adding a CI tool to automate the deploy, but I think is kind of overkill 🔪

### Overall status: Good

**Link(s) to work**

1. [Porfolio](emasuriano.github.io)

## Day 18: February 10, Monday

**Today's Progress**: @disqus successfully implemented in my webpage! Really but really easy with the gatsby-starter 👏

### Overall status: Good

**Link(s) to work**

1. [Porfolio](emasuriano.github.io)
2. [Disqus](https://disqus.com/)

## Day 19: February 11, Thursday

**Today's Progress**: returning to an old project (weather-styled-icon) that I had left it 2 months ago. After so much time, you don't know what's working or not 😕 Time to refactor the whole repo! 😱

### Overall status: Good

**Link(s) to work**

1. [weather-styled-icon](https://github.com/EmaSuriano/weather-styled-icon)

## Day 20: February 12, Friday

**Today's Progress**: I started to code the home/demo page of weather-styled-icon and I realized that the icons that I made weren’t as extensible as I expected (trying to style them was a nightmare) 😣

### Overall status: Regular

**Link(s) to work**

1. [weather-styled-icon](https://github.com/EmaSuriano/weather-styled-icon)

## Day 21: February 13, Saturday

**Today's Progress**: Adding a beautiful color palette from #cooolors to the home page 🎨 Also, I implemented react-github-corner to link to the repository in a great way ✨ Next step upload it to gh-pages 💪

### Overall status: Good

**Link(s) to work**

1. [weather-styled-icon](https://github.com/EmaSuriano/weather-styled-icon)
2. [Palette link](https://coolors.co/e63946-f1faee-a8dadc-457b9d-1d3557)
