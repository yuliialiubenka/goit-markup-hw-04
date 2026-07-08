# goit-markup-hw-04

WebStudio landing page markup and styles for Homework #4. This project continues the page from Homework #3 and adds work with SVG icons, background images, pseudo-elements, transitions, and hover/focus states — while keeping the same semantic HTML, the content container, and the Flexbox layout from the previous homework.

**Project overview**

- **Purpose:** practice working with SVG icons, positioning, transitions, and interactive states based on the provided design.
- **Scope:** a static WebStudio page with header, hero, features, team, portfolio, and footer sections.
- **Assets:** images, the icon sprite, favicon, and all text content are taken from the mockup.

**HTML and CSS structure**

- **index.html** links only to `css/main.css`.
- **main.css** contains only imports of the other style files.
- **CSS files** are split by page parts: `common.css`, `header.css`, `hero.css`, `features.css`, `team.css`, `portfolio.css`, and `footer.css`.
- **Import paths** in `main.css` start with `./`.
- **Common styles** and global rules (`box-sizing`, resets, `.container`, `.section`, `.sr-only`, socials, CSS custom properties) are placed in `common.css`.

**Working with SVG icons**

- Icons are stored in a single sprite and inserted through `<use>`.
- Icon sizes are set in the HTML.
- The `fill` of the social icons is controlled from CSS; the two-color feature icons keep their original colors from the sprite because they are static.
- Social icons are grouped as a list; the size is set on the list item, and the link fills 100% of its parent.

**Transitions and states**

- The `transition` property is set on the base state of an element, not on the hover/focus state.
- All elements that change on hover or focus are animated.
- Buttons and links change color on hover and focus according to the design guide.
- The portfolio overlay slides in on hover over any part of the card, and the card shadow appears on the list item.

**Project requirements covered**

- The project has an `images` folder for graphics and a `css` folder for styles.
- Simple photos are in JPG format, icons are in SVG format.
- File names use only English letters, numbers, and hyphens where needed.
- The code is valid and formatted with Prettier.
- `modern-normalize` is connected in its minified version.
- The layout uses class selectors for styling — no `!important`.
- Unnecessary code and comments are removed.

**Page sections**

- **Header:** logo, navigation with an active-page marker, and contact information in a single container with a bottom border.
- **Hero:** background image with an overlay, a headline, and a call-to-action button.
- **Features:** a visually hidden title and a list of feature items with icon boxes.
- **Team:** team member cards with photos, names, roles, and social media links on a light background.
- **Portfolio:** a section with the `portfolio` id and a grid of project cards with a hover overlay.
- **Footer:** logo, short business description, and a social media block.

**Notes**

- The dominant font is `Roboto`, with `Raleway` used for the logo. Both are connected with a single Google Fonts link.
- Colors and reusable values (radii, shadows, transition) are stored as CSS custom properties in `common.css`.
- Images include size attributes in the HTML.
- The icons are best viewed through Live Server, because external SVG sprites may not load over the `file://` protocol.
