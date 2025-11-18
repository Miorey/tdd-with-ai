---
theme: the-unnamed
colorSchema: dark
layout: cover
background: https://sli.dev/demo-cover.png
---

# Slidev - The Unnamed

Created by [Elio Struyf](https://eliostruyf.com)

---
layout: about-me

helloMsg: Hi!
name: Clement Balea
imageSrc: https://elio.dev/eliostruyf_2024.webp
position: left
job: Software Engineer
line1: "#Stickerpreneur @ pyod.shop"
line2: "#Maintainer @ Front Matter CMS"
social1: "@eliostruyf"
social2: eliostruyf.com
social3: elio@struyfconsulting.be
---

---
layout: cover
---

# Cover title

Subtitle for the cover

<img src="https://wotlk.murlocvillage.com/images/murloc_village_logo.webp" class="mt-6 w-60 mx-auto" />
---
layout: section
---

# Section title

Subtitle for the section

---
layout: center
---

# Center title

Subtitle for the center layout

---
layout: two-cols
---

# Left

This shows on the left

::right::

# Right

This shows on the right

---

# Code with Shiki and The unnamed theme

The code highlighting is powered by Shiki and [The unnamed - VS Code theme](https://marketplace.visualstudio.com/items?itemName=eliostruyf.vscode-unnamed-theme)

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

---

# Table

| Title | Description | Default |
| --- | --- | --- |
| `layout` | The layout to use for the slide | `default` |
| `theme` | The theme to use for the slide | `the-unnamed` |
| `highlighter` | The highlighter to use for the slide | `shiki` |
| `background` | The background to use for the slide | `none` |

## Content test underneath

Some content to place here

---

# Todo

- [ ] Add a todo list
- [ ] Add a todo list
- [x] Add a todo list

---

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

> **Info**: This is a note

---

# What is Slidev?

Slidev is a slides maker and presenter designed for developers, consist of the following features

- 📝 **Text-based** - focus on the content with Markdown, and then style them later
- 🎨 **Themable** - theme can be shared and used with npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embedding Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export into PDF, PNGs, or even a hostable SPA
- 🛠 **Hackable** - anything possible on a webpage

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)


---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel

### Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: image-right
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
---

# Code

Use code snippets and get the highlighting directly!

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

--- 

# Monaco Editor

```ts {monaco}
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

--- 

# Monaco Editor

```ts {monaco-run} {autorun:false}
console.log('Click the play button to run me')
```

---
layout: center
class: "text-center"
---

# Learn More

[Documentations](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)
