# 100 Days Of Code - 2024

## I need to add some context here later, current level of education and skills, why im doing this 100 days and what im hoping to achieve... consistency ect

### Also add a custom git contribution tracker just for this next 100 days !

## Day 1 - 31st May 2024

### Project: Modular Building Construction Company Website

Today, I focused on refactoring the HTML and CSS for a business website I’m building for a friend's modular building construction company.

**Key areas of focus:**

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

**Key areas of focus:**

1. Making the card component reusable for multiple projects
2. Utilizing Flexbox for layout of the seperate elements of the card
3. Using Descriptive Class names


## Day 3 - 2nd June 2024

### Project: My Personal Portfolio Website

Today, I continued working on the card component that will showcase my projects on the "portfolio" page of my personal portfolio website. I was able to reuse most of the HTML and CSS code that I had previuously used in version-2 of my portfolio (This will be version-3 of my Portfolio Website when Im finished :laughing:)

**Key area of focus:**

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

## Day 4 - 2nd June 2024

### Project:

Today, I .

**Key areas of focus:**

1.
2.
3.