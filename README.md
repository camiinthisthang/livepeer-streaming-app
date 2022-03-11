# livepeer-streaming-app
This workshop will walk you through creating a live-streaming web app with Next.js,  Livepeer, and TailwindCSS.

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

3. Ensure everything is working correctly by building your project with the following command in your terminal: ```npm run dev```
4. If you go to ```http://localhost:3000/``` and see something that looks like this, then you're good to go!
<img width="835" alt="Screen Shot 2022-03-11 at 2 45 36 PM" src="https://user-images.githubusercontent.com/15346823/157984567-4b426994-4701-4fa7-a815-c68a4afbd1d6.png">
5. Create a free account with Livepeer and then navigate to the Streams page which you can access [here.](https://livepeer.com/dashboard/streams)
6. Hit ```Create Stream```
![Uploading Screen Shot 2022-03-11 at 3.02.04 PM.png…]()
7. Title your stream, and then you'll be directed to a page with information about your newly created stream, including Stream ID, Stream key, and RTMP ingest URL.
8. Test that your stream is working by using 

