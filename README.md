# Frontend Mentor - Meet landing page solution

This is a solution to the [Meet landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/meet-landing-page-rbTDS6OUR). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements
- interactive to keyboard users

### Screenshot

![](./assets/meet-screenshot.png)



### Links

- Solution URL: [code](https://github.com/ChamuMutezva/typemaster-pre-launch-landing-page)
- Live Site URL: [live site](https://chamumutezva.github.io/typemaster-pre-launch-landing-page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Parcel](https://parceljs.org/) - sass bundler


### What I learned

*** Sass script error *** 
- `sass --watch scss/style.scss:styles/style.css` received the following error even though sass
was installed and showing in the package.json file.

```sass : The term 'sass' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if 
At line:1 char:1
+ sass --watch scss/style.scss:styles/style.css
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (sass:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```
  - Step One  - install sass again using `npm install -g sass`
    try watching sass again on the terminal with `sass --watch scss/style.scss:styles/style.css`
    or just run the following command on the terminal `sass`

    If you get the following error especially for windows users and technically using powershell terminal: 
    ```see about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170.
At line:1 char:1
+ sass --watch scss/style.scss:styles/style.css
+ ~~~~
    + CategoryInfo          : SecurityError: (:) [], PSSecurityException
    + FullyQualifiedErrorId : UnauthorizedAccess
    ```
 - Step Two - Open Windows Powershell as an **adminstrator** 
  on the command line type `Get-ExecutionPolicy -List` to check the execution policy
  On the list look for **Process** and **LocalMachine**
  Execute the following command lines on the terminal
   1. `Set-ExecutionPolicy -Scope LocalMachine Unrestricted` and then accept with a **Y** when requested to do so
   2. `Set-ExecutionPolicy -Scope Process Unrestricted` and accept the changes as well
return to vs code terminal - your sass commands should be ready to go.

- using sass modules @use and @forward and sass inbuilt color- the basic


### Continued development



### Useful resources

- [parcel documentation](https://parceljs.org/) - setting up the project for compilation
- [sass documentation](https://www.example.com) - using modules



## Author

- Website - [Chamu Mutezva](https://github.com/ChamuMutezva)
- Frontend Mentor - [@ChamuMutezva](https://www.frontendmentor.io/profile/ChamuMutezva)
- Twitter - [@ChamuMutezva](https://twitter.com/ChamuMutezva)


## Acknowledgments

Frontend mentor slack community
