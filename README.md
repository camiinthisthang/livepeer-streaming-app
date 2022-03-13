# livepeer-streaming-app
This workshop will walk you through creating a live-streaming web app with Next.js,  Livepeer, and TailwindCSS. Create your own starting from scratch.

### Prerequisites
- Node.js installed 
- Comfortable using the terminal

## Installation and Setup
1. Navigate to the directory where you woud like to store this project. Once you're there create a new Next.js app using by running the following command in your terminal: ```npx create-next-app@latest```

2. Change into your newly created directory with the following command in your terminal: ```cd what-you-named-your-project-in-step-one```

3. Install TailwindCSS into your project. These instructions are copied from TailwindCSS's documentation:
- Install tailwindcss and its peer dependencies via npm, and then run the init command to generate both tailwind.config.js and postcss.config.js. You can do this by running these two commands, one at a time:
```npm install -D tailwindcss postcss autoprefixer ```
```npx tailwindcss init -p```
- Add the paths to all of your template files in your tailwind.config.js file:
```module.exports = {
  content: [
    "./pages/**/*.{js,ts,jsx,tsx}",
    "./components/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
- Add the @tailwind directives for each of Tailwind’s layers to your ./styles/globals.css file:
```@tailwind base;
@tailwind components;
@tailwind utilities;
```

4. Ensure everything is working correctly by building your project with the following command in your terminal: ```npm run dev```

5. If you go to ```http://localhost:3000/``` and see something that looks like this, then you're good to go!
<img width="835" alt="Screen Shot 2022-03-11 at 2 45 36 PM" src="https://user-images.githubusercontent.com/15346823/157984567-4b426994-4701-4fa7-a815-c68a4afbd1d6.png">

5. Create a free account with Livepeer and then navigate to the Streams page which you can access [here.](https://livepeer.com/dashboard/streams)

6. Hit ```Create Stream```
<img width="782" alt="Screen Shot 2022-03-13 at 7 10 30 PM" src="https://user-images.githubusercontent.com/15346823/158081343-37395f23-d02a-49fa-9a5a-4aa23f34a00e.png">

7. Title your stream, and then you'll be directed to a page with information about your newly created stream, including Stream ID, Stream key, and RTMP ingest URL.
<img width="464" alt="Screen Shot 2022-03-13 at 7 10 54 PM" src="https://user-images.githubusercontent.com/15346823/158081361-af7c18d0-220e-44e2-9d39-75383700d340.png">


8. Using a chrome browwer, check that your stream is working by using JustCastIt, a browswer casting by navigating to this link https://justcast.it/to/stream-key-here. Give the page access to your camera and microphone, and hit record.
<img width="137" alt="Screen Shot 2022-03-13 at 7 17 37 PM" src="https://user-images.githubusercontent.com/15346823/158081576-0792c31a-8e06-47d1-9f84-00ea9463a976.png">

9. Back in your Livepeer dashboard from step 7, you should see the feed of your browser livestreaming. 
<img width="473" alt="Screen Shot 2022-03-13 at 7 18 24 PM" src="https://user-images.githubusercontent.com/15346823/158081597-8a05aad7-b97a-480f-9546-9faedfe86425.png">

clone > npm run build > npm start



