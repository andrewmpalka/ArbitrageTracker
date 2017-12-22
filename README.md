
Arbitrage Tracker Project
==========================

[TOC]

Introduction
------------

Hey! Welcome to *Arbitrage Tracker Project*. We're making a web app that leverages the Unofficial Messenger API[^API] to create a *Word Cloud* of a Facebook Messenger thread's chat history for the day. Any contributions to the project are welcome and all will be reviewed. To make a pull request please consult the [Github Documentation][1].

> **Note:** Nothing below is written in stone, it just provides a solid, proven foundation for multiple developers of different skill levels to make impactful contributions to the project. Feel free to make suggestions.

----------


Tech
------

We should strive to make this project both fun and a resume builder for people of all skill levels on the project, so a modern stack is a **must**. The stack that makes the most sense to achieve all these goals is MERN ([**MongoDB**][mongo], [**Express**][express], [**React**][react], [**Node.js**][node]).

> **Note:** This stack is entirely **JavaScript**. If you do not have much knowledge of JavaScript, it's best to check out [Mozilla's excellent tutorials][2].

#### Front-End

As stated above we will be using **React** to display data to the user. If you are not familiar with **React** and want to contribute to the UI, check out [this tutorial][3] by Facebook.

#### Backend
If you don’t have an understanding of **Express**, **Node.js** , **Server-Side JavaScript** check out [this excellent tutorial][4] by Mozilla

> **Note:** Since we have many people working on a project that don't have much experience with JavaScript, we should use [**ES6**][es6] *everywhere* (not only will this be less confusing for newer developers, but desctructuring is awesome).


#### Database

We will be using **MongoDB** and hosting it through [**mLab**][mlab] since anything **NoSQL** is much easier to throw unstructured data at than redis.

> **Note:** Since we have many people working on a project that don't have much experience with **NoSQL**, we will be using a **MongoDB** wrapper called [**Mongoose**][mongoose].

----------


Tools
-------------------

*This section will detail all the suggested tools that will be used over the course of this project.*


#### JavaScript

This project will be using ES6 on the front and back ends for simplicity. We will be following the [**Airbnb Style Guide**][airbnb] and will use their babel preset to keep code uniform. 

> **Note:** To limit the amount of inconsistencies with the linter *and* to have uniform extensions, it would be awesome for all that aren’t very experienced to use the same text editor. [**VS Code** ][vscode] is amazing and since the *.vscode* file will not be included in the *.gitignore*, anyone who pulls down the project and uses **VS Code** will automatically have the same extensions installed by default.

#### Package Management
**Yarn** and **React** go hand in hand, and unless you really like spending the extra 40 or so seconds to install your packages via npm you'll agree. We will be using [**Yarn**][yarn] for this project because there is not a single good reason not to.
>**Note**: We will be using **Node v9.3.0** because of it's tested compatibility with **Yarn**. You can check your node version by opening a terminal window and running
> ```node -v``` 
>If you do not have this exact version, you can easily install it (if you have **nvm** ) by running
>```nvm install 9.3.0
> nvm use 9.3.0``` 

#### Version Control

We will be using Github for this project. If you are unfamiliar with git, github has provided [several tutorials][5] to help you out. If you are new to git, I would advise using a GUI like GitKraken instead of going through the command line. 
>**Note**: If you are using **VS Code** you get an amazing external merge tool right out the the box.

#### Hosting

We will be hosting this project on [**AWS**][aws], while the database will be served via [**mLab**][mlab]
>**Note:** Due to the free-tier of mLab stopping at a very reasonable 500MB we will only store data for a single day and then remove it from memory.

-----

Deployment
-------------

#### TBD
???

------
Getting Started
------------
#### Server
```
cd server && yarn
yarn start
```


#### React App
```
cd app && yarn
yarn start
```


  [^API]: [Unofficial Messenger API](https://github.com/Schmavery/facebook-chat-api#projects-using-this-api) is the only way to automate chat functionalities on a user account. We do this by emulating the browser. This means doing the exact same GET/POST requests and tricking Facebook into thinking we're accessing the website normally.


  [1]: https://help.github.com/articles/creating-a-pull-request/
  [2]: https://developer.mozilla.org/en-US/docs/Learn/JavaScript
  [3]: https://reactjs.org/tutorial/tutorial.html
  [4]: https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs
  [5]: https://guides.github.com/introduction/
  [airbnb]: https://github.com/airbnb/javascript
  [aws]: https://aws.amazon.com/free/
  [es6]: http://es6-features.org/#Constants
  [express]: https://expressjs.com/
  [mlab]: http://mongoosejs.com/index.html
  [mongo]: https://docs.mongodb.com/
  [mongoose]: http://mongoosejs.com/index.html
  [node]: http://mongoosejs.com/index.html
  [react]: https://reactjs.org/
  [vscode]: https://code.visualstudio.com/
  [yarn]: https://yarnpkg.com/en/

