Intro to static site building
-----------------------------
1. How do you connect to `google.com`?
    a. What's in a name?
        - Introduce the recursive nature, e.g. you own everything to the right
        - Get domain names from porkbun, namecheap
        - Avoid country TLDs
    b. Ok, what IP do we point a name at?
        - Github pages (static sites)
        - Free e2.micro on Google Cloud Platform (2 burstable CPUs, 1GB memory, 30GB disk, 1GB network)
        - VPS through Vultr ($5/month, 1CPU, 1GB memory, 25GB disk, 1TB bandwidth), others.
        - Your own server :) (anywhere from $50 to $1000)
    c.
2. Why make your own website?
    - Many many website builders out there (Wordpress, Squarespace, etc)
    - Many "static site generators" like Hugo, Jekyll.
    - Many applications also use HTML/CSS (VSCode, Slack, Obsidian, many video game menus/UIs)
    - Actually knowing the nuts and bolts lets you do whatever you want, even if you use one of these tools.
3. Let's replicate a website!
    - https://www.science.org/doi/10.1126/science.ade9434
    - Introduction to devtools and the inspector
    - What is HTML?
        - A "heavy" markup language.
        - Encodes a tree.
        - Where to look for documentation: [MDN HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) and [MDN CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
        - The [W3 validator](https://validator.w3.org/)
        - DO STEP 01
        - Introduce directly opening file
        - Or with auto-reload
        - `python -m http.server`
4. Breaking down a website into pieces
    - Go top to bottom, left to right.
    - We have some _links_ `<a>`, a `<header>`, some _headings_ `<h1>/<h2>`, and some _paragraphs_ `<p>`, and maybe some `<img>`'s
    - Introduce the fact that `<img>` is a _void tag_.
    - Introduce using `<div>`'s to introduce structure, such as the extra `div` right after the header.
5. Adding style
    - Introduce the [box model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)
    - Introduce the idea of stylesheets and _nested_ selectors.
    - DO STEP 3:
        - Add separate linked CSS file.
        - Start adding CSS classes to elements
        - [CSS selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
        - Start with main_container
        - Move to the abstract and summary
        - Then do the links
    - Introduce [grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout)
        - Add the overall layout columns
    - Introduce [flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
        - Align the top header items.
    - Fix up the breadcrumb links
        - [Styling lists](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Styling_lists)
    - Align the PDF link to the right