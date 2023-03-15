# ![Networky Logo](https://i.imgur.com/0HdJHPd.png) Networky.™ **Turning Acquaintances into Friends.**

**Networky** helps you build and maintain strong relationships with everybody you meet.

Through spaced repetition of social check-ins at customizable intervals, this beautiful web application facilitates the process of turning acquaintances into friends over time, helping you stay relevant in your contacts' lives.

Networky improves your relationships with the people in your life whom provide value to ***you*** by reminding you to periodically provide value to ***them***!

Networky also gives you the power to make your contacts feel ***remembered*** by allowing you to add both a biography and any number of dated notes to each of your contacts, and makes it easy to reach out by bringing all your contact's social links into a single place.

**Learn more below, or check it out here:** [https://networky.io/](https://networky.io/)

![networky](https://user-images.githubusercontent.com/96756923/224582092-c102d165-04b0-447a-ae4b-c45cf10e651f.gif)

<!-- ![networky](https://user-images.githubusercontent.com/96756923/224581524-81909820-9876-4067-a719-c7ae7e8820fd.gif) -->

---

## <img src="https://i.imgur.com/5y8tUJT.png" width="22" height="22" alt="Question mark icon"> Why Networky?
When I first began networking in tech, I would often meet somebody new and then forget to follow up with them in a timely fashion- by the time I finally remembered to reach out again, weeks or months had gone by and neither of us could remember much about the other person- a bit awkward, and not the best start to building a meaningful friendship!

I built Networky to solve this problem once and for all.

---


## <img src="https://i.imgur.com/iloz5JU.png" width="22" height="22" alt="Sparkle icon"> Features of Networky

| *Feature*|*Description*|
|---|---|
| **Contacts** | Contacts can be added, edited, or deleted at any time. |
| **Keep In Touch** | Set a social check-in interval for each contact, and Networky will let you know when your next check-in is due. |
| **Keep It Together** | Networky keeps every personal and professional link for your contacts in one place. Quickly and easily reach out via whichever channel you desire with one click. |
| **Biography and Notes** | Add a biography and dated notes to your contacts, helping you to remember personal details and what you talked about last. |
| **Categories** | Organize your contacts into categories like coworkers, referrals, and friends. You can have any number of categories, and name those categories however you like. |
| **Versatile Sorting** | Sort your contacts by check-in due, alphabetically, by company, and more! |
| **Live Search** | The search function queries name, company, position, biography, and notes to find the person you're looking for instantly. |
| **Customization** | Customize several different options in Settings to make Networky work for you. |
| **Themes** | Networky also includes several beautiful light and dark themes to choose from. |

---

## <img src="https://i.imgur.com/S4sorRH.png" width="22" height="22" alt="Hammer icon"> How It's Made

### <img src="https://i.imgur.com/6QAZVDL.png" width="16" height="16" alt="Eye icon"> **FRONTEND TECH:** React, React-Redux, React-Router, Axios, Date-Fns, Javascript, JSX, CSS


I love working with React, but the necessity of lifting up and drilling down shared state has always felt cumbersome when developing a complex frontend. 

This is why I opted to use Redux to manage the vast majority of my state- specifically the React-Redux toolkit, which made store setup and reducer/action creation easy. I used two main 'slices' of state- one to store user data fetched from the backend, and the other to control the behavior of ui components.

In order to remain true to my initial vision (and because it's fun), I built every component from scratch, and hand coded every line of JavaScript and CSS. The structure and flexibility of my components improved as the project went on as I experimented with more complex props.

React-Router is used to control the display of certain components based on the URL route.

Date-Fns is used to perform calendar-arithmetic and Date() object conversion.

Axios is used to communicate with the backend.


### <img src="https://i.imgur.com/98tktJu.png" width="16" height="16" alt="Eye icon"> **BACKEND TECH:** Node.js, Express, Mongoose/MongoDB, JSON Web Token, BCryptJS, Node Mailer, CORS, Morgan, Validator

Networky's backend is built with Node.js and Express.

The MVC paradigm is used for organization on the backend. Models, Routes, and Controllers are segregated and highly modularized to make understanding and updating the code as simple as possible.

User data is stored in a MongoDB database, using Mongoose to manage the creation and editing of that data.

User session authentication is handled with JSON web tokens, which are verified on every protected CRUD request from the frontend.

User passwords are securely hashed with BCryptJS before being stored in the database.

System emails for new account email verification and password resets are implemented via Node Mailer.

CORS is used to ensure the backend only accepts requests from networky.io.

Morgan is used for server-side logging of requests.

Validator is used to validate user inputs.

---

## <img src="https://i.imgur.com/MUcJhxt.png" width="22" height="22" alt="Speedometer icon"> Statistics

- 290+ hours spent designing, prototyping, coding, refactoring, and polishing
- 120+ issues closed throughout development

### Frontend
- 5,224 lines of JavaScript
- 2,704 lines of CSS
- 1,357 lines of comments (because documenting your code is important!)
- 35 hand built components

### Backend
- 1,397 lines of JavaScript
- 561 lines of comments
- 20 routes
- 20 controllers
- 3 models

---



## <img src="https://i.imgur.com/JwqwRKe.png" width="22" height="22" alt="Speedometer icon"> Optimizations

As time permits, there are several optimizations and improvements that I'd like to integrate into Networky in future updates.

Potential future features/optimizations include:
- Integrate Cloudinary to allow users to upload contact photos themselves
- "Remember Me" option when logging in to disable automatic inactivity logout
- Expandable/Shrinkable contact cards
- Implement React Error Boundary to catch any errors not caught by my custom error handling component
- Allow user to set an "action due" string to be associated with the next check-in date (Examples: "Send thank you email", "Ask how the kid's soccer tournament went", etc)
- Refactor the way the 'uncategorized' category works
- Refactor auth token implementation to be cleaner

---

## <img src="https://i.imgur.com/uOmYnHa.png" width="22" height="22" alt="Speedometer icon"> Lessons Learned

- Familiarized myself with Redux, and with it, many principles of functional programming and the advantages of that paradigm
- Practiced building a complex project with MVC-based architecture, making my backend code more organized and maintainable than ever before
- Practiced building (and organizing) a wide range of components which became more and more versatlie as the project went on
- Learned how to handle authentication via JSON web tokens
- Learned how to effectively connect a React frontend to a Node backend via API requests and token verification
- Learned how to auto-generate and send emails to users via Node Mailer

---

## <img src="https://res.cloudinary.com/dl0htq50i/image/upload/v1678864683/networky-readme_icons/readme_icons-bug_qqiy5p.png" width="22" height="22" alt="Bug icon"> Bug Reports and Feature Requests

To report a bug report or request a new feature, file an issue <a href="https://github.com/ramblingadam/networky-public/issues">here</a>.

---

## <img src="https://res.cloudinary.com/dl0htq50i/image/upload/v1678865846/networky-readme_icons/readme_icons-love_networky_drqogj.png" width="22" height="22" alt="Enjoy networky icon"> Enjoy Networky?

Networky is a thank-you gift to the incredible community of software engineers at 100Devs, and is completely free.

In addition, Networky will never sell or share user data with anybody, ever.

That said, building Networky takes a lot of my time, and keeping it online costs money. Your donation, no matter how small, makes a big impact. Thank you and I hope you enjoy networking with Networky!

<a href="https://www.paypal.com/donate/?business=SBTL552EAS9BU&no_recurring=0&item_name=Help+me+continue+making+innovative+software+solutions.+Your+donation%2C+no+matter+how+small%2C+makes+a+big+impact.+Thank+you%21&currency_code=USD" target="_blank"><img src="https://res.cloudinary.com/dl0htq50i/image/upload/v1678865505/networky-readme_icons/chrome_31o04YZELF_yymbwa.png"></a>

---

## <img src="https://i.imgur.com/SwwiQPj.png" width="22" height="22" alt="Copyright icon"> Copyright & Source Code

All original code in this project is ©Adam Morsa. All rights reserved.

Networky is currently closed-source.

If you are actively recruiting a software engineer, I'd be happy to facilitate a code review. Reach out to me at <a href="mailto:adam@adammorsa.com" target='_blank'>adam@adammorsa.com</a>.

---

## <img src="https://i.imgur.com/GeLZKbH.png" width="22" height="22" alt="Code icon"> Other Projects
Take a look at these other awesome projects from my portfolio!

#

**Magic Task Timer:** [https://github.com/ramblingadam/magic-task-timer](https://github.com/ramblingadam/magic-task-timer)

[![Screenshot of Magic Task Timer](https://user-images.githubusercontent.com/96756923/186636834-a45327e8-90ea-4c34-b3e9-b5e5b1dfdd5b.gif)](https://user-images.githubusercontent.com/96756923/186636834-a45327e8-90ea-4c34-b3e9-b5e5b1dfdd5b.gif)

#

**Animal Crossing: New Horizons Database:** [https://github.com/ramblingadam/acnh](https://github.com/ramblingadam/acnh)

[![Screenshot of ACNH Database](https://user-images.githubusercontent.com/96756923/170849487-39d5a25f-0ad3-4494-a325-d4502610b54e.gif)](https://github.com/ramblingadam/acnh)

#

**X-Wing VS TIE Fighter:** [https://github.com/ramblingadam/tic-tac-starwars](https://github.com/ramblingadam/tic-tac-starwars)

[![Screenshot of X-Wing VS TIE Fighter](https://user-images.githubusercontent.com/96756923/170849366-e1b8d33b-6236-46f1-8dd9-b38fd2c27380.gif)](https://github.com/ramblingadam/tic-tac-starwars)
