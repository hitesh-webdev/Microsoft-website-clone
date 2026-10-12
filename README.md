# Microsoft Homepage Clone

🔗 **Live Demo:** [View Website](https://exquisite-cobbler-a7df3a.netlify.app/)

A responsive recreation of the Microsoft homepage, built with **pure HTML5 and CSS3**. No JavaScript, no frameworks.

I built this as a hands-on practice project to learn how a complete webpage is put together, and then made the layout work across desktop, tablet and mobile screens using media queries.

> **Disclaimer:** This is a learning project and is not affiliated with or endorsed by Microsoft. All logos, images and trademarks belong to Microsoft Corporation.

## Overview

The page recreates the main sections of the Microsoft homepage:

- Navigation bar (logo, links, search, cart, profile)
- Hero banner with call-to-action
- Quick-link categories (Microsoft 365, Xbox, Windows 11, Surface)
- Product card section
- Feature and sustainability banners (text and image side by side)
- "For business" card section
- Social media links
- Six-column footer

## Tech Stack

- **HTML5** for page structure
- **CSS3** for layout, styling, hover effects and responsiveness
- [**Font Awesome 6**](https://fontawesome.com/) for icons

## Concepts Practiced

**Flexbox** is used for most of the layout: the navbar, product and business cards, feature and banner sections, social links and footer. Properties like `justify-content`, `align-items`, `gap`, `flex-direction` and `flex-wrap` work together through parent-child relationships.

**Positioning and image handling.** The hero text is placed over the background image using `position: absolute`, and images use `object-fit: cover` so they fill their containers without stretching.

**Hover effects.** Cards get a soft `box-shadow` on hover, and navigation and footer links get an underline with a custom `text-underline-offset`.

**Media queries.** Multiple breakpoints adapt the layout from large desktops down to small phones.

## Responsive Design

The desktop layout is the base. Responsiveness is added with media queries at the end of `style.css`, so the original styles stay intact.

| Screen width     | What changes                                                                   |
| ---------------- | ------------------------------------------------------------------------------ |
| above 1400px     | Full desktop layout                                                            |
| 1400px and below | Navbar labels (Search, Cart, Sign in) hide, only icons remain                  |
| 1300px and below | Page height adapts to content, cards wrap, feature and banner layouts simplify |
| 1100px and below | Windows, Surface, Xbox and Support links hide from the navbar                  |
| 1000px and below | Cards switch to 2 per row                                                      |
| 900px and below  | Feature and banner sections stack vertically                                   |
| 700px and below  | Quick links go 2 per row, footer columns narrow                                |
| 600px and below  | Simplified navbar (logo, search, cart, profile)                                |
| 420px and below  | Footer becomes a single column                                                 |

## Challenges I Faced

- **Matching an existing design.** Recreating a real interface needs much more attention to spacing, sizing and alignment than building a layout from scratch.
- **Making the layout responsive.** Some desktop dimensions needed to be adjusted at smaller screen sizes, so I had to work out which properties to override at each breakpoint so the page could grow with its content.
- **Text positioned over an image.** The hero text had to stay readable and well placed as the image shrinks, so it needed a different layout on smaller screens.
- **Keeping the navbar clean.** Deciding which links and labels to hide at each screen size so the navbar never overflows.

## What I Learned

- Structuring a complete webpage with HTML
- Using Flexbox to build and align components
- Controlling spacing with `margin`, `padding` and `gap`
- Writing media queries and thinking in breakpoints
- Handling images with `object-fit`
- Building hover feedback with CSS alone
- Understanding how properties interact with the page structure, not just knowing them individually

## Project Structure

```text
.
├── Index.html   # Page markup
├── style.css    # All styles, including responsive media queries
└── README.md
```

## Notes
- Images are loaded directly from Microsoft's CDN, so you need an internet connection to see them.
- Icons come from the Font Awesome CDN.

Future Improvements
- Mobile navigation menu (hamburger) for small screens
- Working links and a functional search
- Accessibility improvements (better alt text, keyboard navigation)
- Self-hosted images for faster loading

Acknowledgement
Thanks to my mentor, Devendra Dhote, for the guidance and feedback while I was learning frontend development.

Author
Hitesh Verma
- GitHub: [@hitesh-webdev](https://github.com/hitesh-webdev)

License
This project is for educational purposes only.
