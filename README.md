## Sections

✔️ Summary and About me\
✔️ Skills \
✔️ Open Source Projects Connected with Github\
✔️ Big Projects\
✔️ Contact me

## Getting Started 🚀

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

You'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer or use [Docker](https://www.docker.com/products/docker-desktop).

```
node@v10.16.0 or higher
npm@6.9.0 or higher
git@2.17.1 or higher
```

### Docker Commands

```
1) BUILD IMAGE : docker build -t developerfolio:latest .
2) RUN IMAGE: docker run -p 3000:3000 developerfolio:latest
```

## How To Use 🔧

From your command line, clone and run tarunPortfolio:

```bash
# Clone this repository
$ git clone

# Go into the repository
$ cd tarunPortfolio

# Install dependencies
$ npm install

```

## Github Setup For Open Source Projects

### Generate a Github personal access token using these [Instructions](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) `Make sure you don't select any scope just generate a simple token`

Copy the token and open Chrome Developer Console to convert your token to base64 so github do not revert your token when you push your token to git

```bash
# Open your Chrome Developer Console console paste the token inside btoa
$ btoa("YOUR GITHUB TOKEN")
```

Copy your converted token and paste it in `/src/portfolio.js`

```javascript
  const openSource = {
  /* Your Open Source Section to View Your Github Pinned Projects */
  /* To know how to get github key look at readme.md */

  githubConvertedToken: "Your Github Converted Token",
  githubUserName: "Your Github Username"
  showGithubProfile :"true" // Set true or false to show Contact profile using Github, defaults to false
};
```

For the GitHub profile, set true or false to show Contact profile using Github, defaults to false.

## Change and customize every section according to your need.

### To Change website content go to `/src/portfolio.js` & modify it as per your need.

#### Using Emojis

For adding emoji 😃 into the texts in Portfolio.js, use the `emoji()` function and pass the text you need as an argument. This would help in keeping Emojis compatible across different browsers and platforms.

```javascript
/* Change this file to get your Personal Porfolio */

const greeting = {
  /* Your Summary And Greeting Section */
  title: "Hi all I'm Tarun Tyagi",
  subTitle: emoji("A passionate Full Stack Software Developer 🚀"),
  resumeLink: "https://www.keepandshare.com/doc28/110137/tarun-pdf-142k?da=y"
};

const socialMediaLinks = {
  /* Your Social Media Link */
  github: "https://github.com/Taruntyagi93",
  linkedin: "https://www.linkedin.com/in/tarun-tyagi-018a4549/",
  gmail: "taruntyagi0193@gmail.com",
  facebook: "https://www.facebook.com/tarun.tyagi.58118",
  twitter: "https://twitter.com/taruntyagi93",
  instagram: "https://www.instagram.com/taruntyagii/",
};


const skillsSection = { .... }

const techStack = { .... }

const openSource = { .... }

const bigProjects = { .... }

const achievementSection = { .... }

const blogSection = { .... }

const contactInfo = { .... }

const twitterDetails = { ... }

```

#### Adding Twitter Timeline to your Page

Insert your Twitter username in `portfolio.js` to show your recent activity on your page.

```javascript
const twitterDetails = {
  userName: "Your Twitter Username",
};
```

Note: Don't use `@` symbol when adding username.

## Technologies used 🛠️

- [React](https://reactjs.org/)
- [graphql](https://graphql.org/)
- [apollo-boost](https://www.apollographql.com/docs/react/get-started/)
- [react-twitter-embed](https://github.com/saurabhnemade/react-twitter-embed)
- [react-easy-emoji](https://github.com/appfigures/react-easy-emoji)
- [axios](https://github.com/axios/axios)
