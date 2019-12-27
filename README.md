<a href="https://significa.co"><img src="https://user-images.githubusercontent.com/4838076/70076649-20d29b00-15f7-11ea-9379-e2fa1889a525.png" alt="logo" width="300px"></a>

![](https://github.com/significa/significa.co/workflows/Deploy%20to%20Production/badge.svg)

This is the repo for [Significa's website](https://significa.co/), our very own presence on the web.

![significa.co cover](https://user-images.githubusercontent.com/5202712/71517795-96085780-28a7-11ea-8a6b-ee9b402d6ac4.png)

## significa.co

Project built with Gatsby. You can find more information on available scripts at https://www.gatsbyjs.org/.

### Start up the project

Start a local development server at http://localhost:8000/

```sh
npm run develop
```

### Build

Make a new build to `/public` folder

```sh
npm run build
```

### Run storybook

Start [storybook](https://storybook.js.org/) server to develop components in isolation

```sh
npm run storybook
```

### Validate codebase

Run prettier, eslint, typescript and jest to validate codebase

```sh
npm run validate
```

## Lambda functions

### Prerequisites

- Make sure you have [aws cli](https://aws.amazon.com/cli/) installed in your machine.
- Run `aws configure` to setup a user with access to Significa's AWS
- These lambdas' region is Ireland (`eu-west-1`)

### Deploy new version

To deploy a new lambda version you need to first navigate to the directory

```
cd functions/contact
```

install dependencies

```
npm install
```

and then run the script to build, zip and deploy

```
npm run deploy
```

check `package.json` on each function for more available scripts
