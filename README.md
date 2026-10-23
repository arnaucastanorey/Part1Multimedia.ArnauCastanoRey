# Part1Multimedia.ArnauCastanoRey

# Arnau Castaño – CV Website

This is my CV website for the Hypermedia project (Part 1). It is a single-page static website made with HTML and CSS. I designed it first in Figma and then I built it in Visual Studio Code.

- **Figma:** [CV Template](https://www.figma.com/design/OnKmlDjZD7LuglJTuWZr3k/CV-Template?t=6q8Pc0DI2rYcGN38-1)

## 1. Project analysis

### 1.1 User profile

Name: Marc Roca (fictional)
Age: 34
Job: Lead programmer in a small indie video game studio (8 people)

Marc programs every day, but when the studio needs a junior programmer or a student for an internship, he is the one who reads the CVs. He wants to be sure that the person knows the basics before the team loses time with an interview. He does not have much time. He reads CVs in the breaks between coding sessions, and he decides in around one minute if he wants to know more about the person.

**What does he want to find?**

- What the person studies, and if it is related to game design or development.
- Which tools and programming languages the person knows (for example C++, JavaScript, HTML, CSS, Matlab, Visual Studio Code and Photoshop).
- What the person likes (for example 3D design and animation), to see if he fits with the type of games the studio makes.
- Some work experience, even if it is not about games, because it shows that the person is responsible.
- A clear way to contact the person (email and phone).

**What problems does he have?**

- Many CVs say "I am good at programming" but they do not say which tools or languages.
- Some CVs are too long, or they have too much text and are difficult to read.
- Sometimes it is hard to find the contact information.

**What does he need from my website?**
A clean page where he can see my studies, my tools and my contact details quickly, with the tools shown as logos so he understands them in one look.

### 1.2 Information architecture

My website is one single page and the information goes from the most general to the most detailed. I used four parts, from top to bottom.

1. **Presentation.** This is the first thing that the user sees. It has my name in a very big size, my title ("Videogames Designer & Developer"), a small tag that says "Studying", a short introduction and my photo. I put my languages in a small card on top of the photo, so the user can see them quickly without looking for them.
2. **About me.** Here I wrote a short text about who I am and what I like (3D design, animation and programming). On the right side I put my personal details: date of birth, city, email and phone number. I put them next to the text because a person like Marc needs the contact information fast, and they are easy to find in a dark section with icons.
3. **Formation, Skills and Experience.** These three parts are in three columns, one next to the other, inside one big rounded box. The user can compare them in only one look.
   - **Formation:** my studies, from the newest to the oldest one.
   - **Skills:** the tools with their logos, because logos are faster to read than words.
   - **Experience:** my jobs, also from the newest to the oldest.

   Each item always has the same order: title, date and place.

### 1.3 Visual design

**Inspiration.** I looked for CV websites and templates on Pinterest to get ideas. Many of them used a simple layout, a lot of empty space and only one or two colors. I liked that style, so I used these ideas and I made my own design from zero in Figma.

**Colors.** I used a limited color palette so the page looks clean:



Dark blue-black `#14181c`. Dark sections and the footer 

Teal / turquoise `#17b7b0`. Main accent: small titles, icons and the line under "I'm Arnau!" 

Dark teal `#0e8a85`. My job title 

Beige `#f5f3ef`. Light background (softer for the eyes than pure white) 

Light blue `#cee8eb`. Languages card, so it stands out from the beig

Grey `#6b6b66`. Small texts such as dates and places

The page changes between light and dark parts. This helps the user to see where one section ends and the next one starts.

**Typography.** I used three fonts from Google Fonts so they can be the same as in Figma:

- **Playfair Display (bold)** for my name and for "I'm Arnau!". It is an elegant serif font and it gives personality to the page.
- **Platypi (bold)** for my job title, because it goes well with Playfair but it is a bit different.
- **Inter** for the rest of the text. It is a sans-serif font that is very easy to read on a screen, even when the size is small.

I used big sizes for the titles and small sizes for the details, so the user knows what is more important.

---

## 2. Tools and technologies

- **Figma** – to design the page before coding.
- **Visual Studio Code** – to write the code.
- **HTML and CSS** – the website itself.
- **Google Fonts** – for the typography (imported with `@import` in the CSS file).

---

## 3. Files of the project

File Description 

`FigmaCV.html`. The structure and the content of the page. 
`FigmaCV.css`. All the styles (colors, fonts, layout). 
Image files. My photo, icons and tool logos.

## 4. Problems I found and how I solved them

- **Floating columns.** The three columns of the third section use `float`. At the beginning, the footer was hidden behind them, because a parent does not grow when its children float. I solved it by putting the columns inside a `div` with `overflow: hidden`.
- **Same height in the columns.** The three columns had different heights. I set the same height to all of them so it looks like the Figma design.
- **Typography.** The fonts did not look like the ones in Figma at first. I solved it by importing them from Google Fonts with `@import`.
- **Zoom in the browser.** The page looked different when my browser zoom was not 100%. I learned to check it before comparing with Figma.
- **Logo of JavaScript in the wrong place.** The first row of tools has five logos, but the fifth one (JavaScript) went to the second row. The reason was that every logo has a `margin-right` of 16 px, even the last one, and then the five logos did not fit in the width of the column. I solved it by removing the margin of the last logo with `:last-child`.
