# 100 Days Of Code - 2024

## I need to add some context here later, current level of education and skills, why im doing this 100 days and what im hoping to achieve... consistency ect

### Also add a custom git contribution tracker just for this next 100 days !

## Day 1 - 18th June 2024

### Project: My Personal Portfolio Website

Today, I have started back working on my personal portfolio website v3 that I've been procrastinating on for a while.

I had an issue with the Theme toggler code I had written, it worked fine on the home page where I was also updating the theme of my github stats card but on the other pages were this element didn't exist the variable that refrences that HTML elemement was returning null creating a runtime error. To fix this I implemented a guard clause if (githubStatCard !== null) to check that the Github Stats Card is an element within the current page if not the code to change the Src attribute is not ran.

I also refactored some of the functions I use to toggle the theme, I had some if else statements that I decide to make more concise with ternary statements:

Previous Code:

function toggleTheme() {
  if (theme === 'dark-theme') {
        theme = 'light-theme';
  } else {
        theme = 'dark-theme';
    }
}

Refactored with Ternary Operator:

function toggleTheme() {
    theme === 'dark-theme' ? theme = 'light-theme' : theme = 'dark-theme';
}


**Key Areas of Focus:**

1. JavaScript
2. Guard Clauses
3. Ternary Operators


### Additional Activities:
--





----------------------------------
# My First Attempt at #100 days of code, after missing a few days have decided to restart on the 18th of June


## Day 1 - 31st May 2024

### Project: Modular Building Construction Company Website

Today, I focused on refactoring the HTML and CSS for a business website I’m building for a friend's modular building construction company.

**Key Areas of Focus:**

1. Using semantically correct HTML elements
2. Implementing a mobile-first design approach
3. Utilizing Flexbox for layout
4. Writing concise CSS with minimal duplication

### Additional Activities:

- Started reading the eBook *Ten Ways to Make Money as a Developer* by Florin Pop (read for 30 minutes)


## Day 2 - 1st June 2024

### Project: My Personal Portfolio Website

Today, I have started back working on my personal portfolio website v3 that I've been procrastinating on for a while.
The section I was focused on was building a card component to be used on the portfolio page of the website to showcase some of my personal projects and previous work.

**Key Areas of Focus:**

1. Making the card component reusable for multiple projects
2. Utilizing Flexbox for layout of the seperate elements of the card
3. Using Descriptive Class names


## Day 3 - 2nd June 2024

### Project: My Personal Portfolio Website

Today, I continued working on the card component that will showcase my projects on the "portfolio" page of my personal portfolio website. I was able to reuse most of the HTML and CSS code that I had previuously used in version-2 of my portfolio (This will be version-3 of my Portfolio Website when Im finished :laughing:)

**Key Areas of Focus:**

1. Making the project text description section of the cards expandable with a “Read Full Description / Show Less” toggle. This leads to a cleaner UI and an improved UX, giving users the choice to view the full description or not. I achieved this functionality with just HTML and CSS by using a checkbox as a button, setting custom CSS variables for the line height and the maximum number of lines shown, and using CSS calc, overflow: hidden, and the ::before and ::after pseudo-classes.

I've included some CSS code snippets below:

```
.project-description {
    font-size: 16px;
    margin: 16px 0 0 0;
    line-height: 1.1;
}

.cutoff-text {
  --max-lines: 3;
  --line-height: 1.25;
  padding: 0;
  height: calc(var(--max-lines) * 1em * var(--line-height));
  line-height: var(--line-height);
  overflow: hidden;
}

.expand-btn {
  border: none;
  appearance: none;
  outline: none;
  width: 240px;
  font-size: 12px;
  padding: 0;
  color: white;
  letter-spacing: 1.8px;
}

.expand-btn::before {
  font-family: "Font Awesome 5 Free";
  content: "Read Full Description \f078";
}

.expand-btn:checked::before {
  content: "Show Less \f077";
}

.cutoff-text:has(+ .expand-btn:checked) {
  height: auto;
}
```

### Additional Activities:

- Continued reading the eBook *Ten Ways to Make Money as a Developer* by Florin Pop (read for 20 minutes)

## Day 4 - 3rd June 2024

### Project: My Personal Portfolio Website

Today, I continued working on the card component that will showcase my projects on the "portfolio" page of my personal portfolio website.

**Key Areas of Focus:**

1.	Moving hoverable state CSS declarations into a media query for hoverable devices.
2.	Updating the card color scheme to align better with the other pages and components of the website. I used CSS custom variables that were already in use elsewhere on the site, ensuring that the card components’ colors change to match the rest of the theme when the user toggles between dark and light modes.


## Day 5 - 4th June 2024

### Project: Modular Building Construction Company Website

Today, I focused on writing the CSS declarations for the responsive design for desktop screen sizes on the main homepage sections. Additionally, I decided to simplify the current header and nav bar. Initially, I had integrated a hero section into the header, with plans to display images in a timed loop and include pagination. However, this design did not aesthetically fit with the rest of the site. To avoid delays in launching the website, I decided to create a more basic MVP and will improve on it further in the future.

**Key Areas of Focus:**

1. Responsive Design - Utilizing Flexbox for layout
2. Header and Nav Structure - Building and refactoring the structure, and styling it appropriately for the user’s viewport.
3. Figma - Working from a Figma wireframe, Doing my best to match the wireframe 100%


## Day 6 - 5th June 2024

### Project: My Personal Portfolio Website

Today, I had only one hour to spare due to other commitments. However, I am committed to maintaining at least one hour of coding or studying programming every day for 100 days. So, I made sure to sit down and get it done :muscle:

I focused on the contact form page. A couple of months ago, I wrote the basic HTML structure for the form, so I spent my time familiarizing myself with the code and started applying CSS styling to the form wrapper, input fields, and the submit button. My goal is to make the contact form as modular and reusable as possible, as I have other websites I’m currently working on and would like to reuse a good portion of this code to speed up my workflow.

**Key Areas of Focus:**

1. HTML Forms
2. Responsive Design - Mobile First


## Day 7 - 6th June 2024

### Project: My Personal Portfolio Website

Today, I continued styling my contact form and added client-side JavaScript validation for inputs before allowing form submission. I’m satisfied with my validation functions as they achieve the desired result, but I’m already considering ways to refactor them for improved modularity and conciseness. Additionally, I focused on creating and styling error states for when the form fails validation, such as when a name is not supplied, the email address doesn’t match the standard pattern, or the message text hasn’t reached the minimum character count.


**Key Areas of Focus:**

1.	JavaScript - Writing functions to validate user input before submitting the form to the server.
2.	UI/UX Design Principles - Designing user hints and error states.
3.	JavaScript - Adding and removing CSS classes to UI elements based on form validation success or failure.
4.	CSS - Styling error states, warning icons, and user hints/messages to indicate what requires attention before submission can be completed.

### Additional Activities:

- Continued reading the eBook *Ten Ways to Make Money as a Developer* by Florin Pop (read for 20 minutes)
- Discovered the Coding Sloth YouTube channel, which appears to be a fantastic learning resource. Watched one of his videos on the importance of logical and problem-solving thinking as a developer.
- Signed up for a 28-day trial on Brilliant.com to explore their interactive courses on coding, computer science, data structures, and algorithms. I’ve studied DSA before but could definitely use a refresher.


## Day 8 - 7th June 2024 & Day 9 - 8th June 2024

### Learning Platform: Brilliant.com

Limited amount of spare time on these 2 days but have started the brilliant.org CS & Programming Learning Path to refresh and further develop skills in programming and algorithmic thinking.

Currently working through Level 1.1 - Thinking In Code

It doesnt cover a specific language, but the thought process and foundations for computational problem solving. The concepts and logical way of thinking is something I feel quite familiar with so it has been easy for me to complete the lessons. I really am enjoying the refresher though and the way they teach the concepts on the "brilliant platform" its very interactive and explains the concepts in a much more relatable way then some of the other introductory courses I'd taken a couple of years ago.

**Key Subjects of Learning / Revision:**

1. Computational Problem Solving
2. Writing Basic Programs
3. Loops & While Loops
4. Recognizing Patterns


## Day 10 - 9th June 2024

### Learning Platform: Brilliant.com

Today, I continued on with the CS & Programming Learning Path on Brilliant.com


**Key areas of Learning / Revision:**

1. Practice Recognizing Patterns
2. Using Conditional Statements


### Additional Activities:

- Continued reading the eBook *Ten Ways to Make Money as a Developer* by Florin Pop (20 minutes)
- Created a Notion Document to take notes of the most important takeaways from my reading of *Ten Ways to Make Money as a Developer* (30 minutes)



## Day 11 - 10th June 2024

### Project: My Personal Portfolio Website + Continued CS & Programming Learning Path on Brilliant.com

Today, I made several improvements to my portfolio website:

- Contact Form Alignment: Adjusted the contact form alignment for larger desktop viewports to ensure a more polished look.
- Text Area Enhancements: Improved the user experience of the text area by setting textarea {resize: none} and increasing its default height using the rows attribute. This prevents users from needing to scroll up after writing just three lines. I plan to further research how to enable dynamic resizing when users input more than nine rows of text.


I continued on with the CS & Programming Learning Path on Brilliant.com:

I've recently started on the Brilliant platform (free 1 month trial) and this course so its revision of concepts I have a very good grasp of already but am finding it good to go over the fundamentals again as its sparking the odd new insight and reinforcing my understanding of core programming principles. Todays Revision Topics Were:

**Conditional Statements:**
- Purpose: Used primarily for decision-making and control flow within programs, allowing different actions based on conditions.
- Benefits: Simplifies complex logic into manageable steps, making code more readable and maintainable.

**While Loops:**
- Usage: Ideal for repeatedly executing a block of code as long as a condition is true, especially when the number of iterations is unknown.
- Benefits: Automates repetitive tasks, increasing efficiency and reducing manual intervention.


**Key areas of Focus / Learning / Revision:**

1.	UI/UX Design Principles
2.	Textarea HTML Element - available attributes and styling

3. Conditional Statement Fundamentals
4. While loop Fundamentals


### Additional Activities:

- Continued reading the eBook *Ten Ways to Make Money as a Developer* by Florin Pop (25 minutes)


## Day 12 - 11th June 2024

### Learning Platform: Brilliant.com

Unfortunatley I didnt manage my time very well today and was disappoionted with the little time and effot I did manage to commit to my #100 days of Code Journey. Today consisted of some further revison and practice challenges related to Conditional Statements and While loops and also 25 minutes of Reading of *Ten Ways to Make Money as a Developer* by Florin Pop (25 minutes)

Moving forward I hope to have much better focused days as achieving consistency with my studies and daily coding is something that is super important to me.


## Day 13 - 12th June 2024

### Project: My Personal Portfolio Website + Continued CS & Programming Learning Path on Brilliant.com

Today, I made several improvements to my portfolio website:

- 
-


I continued on with the CS & Programming Learning Path on Brilliant.com:

Todays Revision Topics Were:

**Combining multiple Conditional Statements and nested loops** to solve more complex problems by enabling detailed control over program flow and iteration processes, making it possible to handle intricate problems effectively.


**Key areas of Focus / Learning / Revision:**

1.	UI/UX Design Principles
2.	Textarea HTML Element - available attributes and styling

3. Conditional Statement Fundamentals
4. Nested Loop Fundamentals


### Additional Activities:

- Continued reading the eBook *Ten Ways to Make Money as a Developer* by Florin Pop (25 minutes)



