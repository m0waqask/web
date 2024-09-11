# React
Below will be the notes Im gonna make on each class.

# Class 1
### Whats a DOM?
DOM, or Document Object Model, is like the blueprint for your webpage. Think of it like a puppet show:

HTML: The puppets (your content).
CSS: The clothes and style of the puppets.
JavaScript: The puppet master pulling the strings.
DOM: The stage layout, the rules of the show, and how the puppets move and interact with each other.
When you mess with the DOM, you’re telling the puppet master (JavaScript) to change something on stage—like making a puppet dance or changing its costume (the content and layout of your page). Every time you click something or trigger an event, JS is like, "Yo, DOM, we need a quick change!" The DOM makes that change happen on the page without refreshing the whole damn thing.

So, in simple terms: The DOM is the behind-the-scenes system that lets JS update and interact with your webpage in real-time.

### Why React is better than plain old HTML/CSS/JS:
Component-based: React breaks down the page into little chunks (components) you can reuse, like LEGO blocks, instead of building a whole damn new thing every time.
Efficient updates: Instead of reloading the entire page, React only updates the parts that need to change—no full-page refresh BS.
Cleaner code: React keeps things organized. If your project is big, it’s easier to manage with React, so you don’t end up with a chaotic mess of HTML/JS.
Better performance: React’s virtual DOM (it’s like a faster, fake version of the real DOM) lets it update the page quickly without slowing everything down.
Easy to debug: React shows you exactly what component has an issue, making it easier to fix.
Community support: Tons of developers use React, meaning there are tons of resources, plugins, and libraries to help you get shit done faster.

So yeah, React isn’t just a buzzword—it’s a better way to handle bigger, dynamic websites.

### **Create React App (CRA)**
- **What it is**: The basic of React app setup tools. You run one command, and boom—everything's ready for you.
- **Pros**: 
  - **Simple AF**: Perfect for beginners who don’t want to deal with config files and headaches. 
  - **Pre-configured**: Everything is set up for you—Webpack, Babel, etc.
- **Cons**: 
  - **Slow as hell** for larger projects. CRA drags its feet when things get more complex.
  - Not very flexible, so if you want to customize stuff, you might hit a wall.

### **Vite**
- **What it is**: The cool new kid in town. It’s a build tool that's faster and leaner for modern projects.
- **Pros**: 
  - **Blazing fast**: Development server starts in milliseconds. Unlike CRA, it doesn't choke when your project gets big.
  - **Optimized builds**: It’s all about speed—both in development and production.
  - **Supports modern features**: It plays well with the latest JavaScript features without needing hacks.
- **Cons**: 
  - **Slightly more complex setup**: If you're a noob, you might scratch your head a bit during setup, but once you figure it out, it’s smooth sailing.

In short: If you’re just starting out, **CRA** is fine for small projects. But if you’re building something bigger or more complex, **Vite** will save you a ton of time and frustration by being faster and more efficient.

### **Setting Up the Environment: The React Party Prep**
1. **Install Node.js**: Go to [nodejs.org](http://www.nodejs.org) and download that bad boy. Once installed, run `node -v` and `npm -v` in your terminal to make sure they’re good to go. If they don't work, you probably fucked something up.

2. **Install VS Code**: Grab it from [code.visualstudio.com](http://code.visualstudio.com). This is your code editing hub. Add some swag with extensions like **ESLint** (to catch your dumb mistakes), **Prettier** (to make sure your code doesn't look like garbage), and **React snippets** (because typing the same thing 100 times is a waste of your life).

---

### **Creating a React Project: Your Way In**
1. **Using Create React App (CRA)**:
   - In your terminal, run:  
     `npx create-react-app my-app`  
     Replace `my-app` with whatever name your heart desires. 
   - Navigate to the project folder:  
     `cd my-app`
   - Start the development server:  
     `npm start`  
     And boom, React is up and running.

2. **Using Vite** (the faster, cooler way):
   - In your terminal, run:  
     `npm create vite@latest`
   - Follow the prompts—it’ll ask a couple of questions.
   - Navigate to the project folder:  
     `cd my-app`
   - Install dependencies:  
     `npm install`
   - Fire up the development server:  
     `npm run dev`  
     Now you’re flying with Vite, aka the "speed demon" of React setups.

---

### **Vite Project Structure: What’s What**
- **index.html**: The main HTML file. This is where the show starts.
- **src/**: Your code lives here.
- **main.jsx**: The *bouncer*—this guy lets React into the club.
- **App.jsx**: The main **App** component. This is where you’ll do most of your work.
- **vite.config.js**: The brain of Vite. It’s the configuration file that makes everything tick.

---

### **Why Vite?**
1. **Faster Development**: The dev server is quick AF, and it uses **hot module replacement**, meaning you make a change, and it updates instantly without reloading the whole page.
2. **Optimized Build**: Vite uses **Rollup**, which results in smaller, more efficient production builds. No bloat, just the goods.
3. **Modern Features**: Supports the latest and greatest JavaScript features right out of the gate. You don't have to waste time configuring it—it’s ready to rock.

In short: **CRA** is the beginner-friendly training wheels, while **Vite** is the turbocharged ride for those who want **speed** and **modern tech**.
