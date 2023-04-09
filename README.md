# Gift recommendation - React Native app

This mobile app generates gift recommendations using [React Native](https://reactnative.dev/) and [Expo](https://docs.expo.dev/tutorial/introduction/). The backend is built using the [Next.js](https://nextjs.org/) framework and utilizes the [OpenAI API](https://platform.openai.com/docs/quickstart) for generating gift ideas.

Users can input the characteristics of the person they want to send a gift to and click the 'Generate Gift Ideas' button. The front-end sends requests to a instance deployed on AWS, which then calls OpenAI's API and returns the generated results to the front-end.

Using AWS to fetch data provides an added layer of security for the OpenAI API Key and makes it more convenient for users to get gift recommendations.

## Author

Name: Monica Zhang

UPI: yzhb603

Student ID: 776742548

## How to Install and Run the App

1. If you don’t have Node.js installed, [install it from here](https://nodejs.org/en/) (Node.js version >= 14.6.0 required)

2. Open a new terminal and clone this repository

   ```bash
   $ git clone https://github.com/UOA-CS732-SE750-Students-2023/cs732-se75-assignment-Monica-Zhang-git.git
   ```
3. Open the file

   ```bash
   $ cd cs732-se75-assignment-Monica-Zhang-git 
   ```

4. Install the requirements

   ```bash
   $ npm install
   ```

5. Run the app

   ```bash
   $ npm start
   ```

You should now be able to access the app through a Expo Go App.

1. Download a [Expo GO App](https://apps.apple.com/app/apple-store/id982107779).

2. Choose a device in the terminal according your needs.

   ```bash
   › Press i │ open iOS simulator
   › Press w │ open web
   ```

3. You could Scan the QR code that showed in the terminal with the Camera app(ios) or Expo Go (Android).

## How to Use the App

This application consists of three main pages: the input page, the loading page, and the results page.

<p algin="center">
<img src="https://github.com/Monica-Zhang-git/Img/blob/main/main.png" width=30% >
<img src="https://github.com/Monica-Zhang-git/Img/blob/main/loading.png" width=30% >
<img src="https://github.com/Monica-Zhang-git/Img/blob/main/results.png" width=30% >
</p>

On the input page, users can enter the characteristics of the person they are buying a gift for, including their age, gender, the price range of the gift, and their hobbies. Once the user has entered this information, they can click the 'Generate Gift Ideas' button to begin the gift recommendation process.

Next, the user is taken to the loading page, where they will wait for the gift recommendations to be generated.

Once the recommendations are ready, the user is automatically redirected to the results page, where they can view the gift recommendations.

If the user wants to generate new gift ideas, they can click the 'Try Again' button to go back to the input page and start over.
