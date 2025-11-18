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
---

---
layout: section
---

# Section title

- Subtitle for the section
- Subtitle for the section
- Subtitle for the section
- Subtitle for the section
- Subtitle for the section
- Subtitle for the section

---
layout: center
---

# Center title

Subtitle for the center layout

---
layout: two-cols
---

# Testing Pyramid
![alt text](./assets/pyramid.png)

::right::

# Tools
 <br /> <br /> <br /> <br /> <br /> 
- **E2E:** Cypress · Playwright · Selenium <br /> <br />
- **Integration:** Postman with Newman<br /> <br />
- **Unit:** coverage · SonarQube

---
layout: section
---

# Code
<br />
```py
def plus(val_1: int, val_2: int) -> int:
    return val_1 + val_2
```

<br />
<br />

# Unit Test
<br />
```py
def test_plus():
    assert 3 == plus(1,2)
    assert -1 == plus(1,-2)
    assert -3 == plus(-1,-2)
```
 
---

# Example 1: generate tests and modify code

- Generate tests for a function with LLM
- The test coverage shows us the uncovered lines ex we add:
```py
    elif last_name == "Summers":
        ret = "Buffy Summers" 
```
- Rewriting function without regressions ex:
```py
def find_full_name_v1(last_name: str) -> str | None:
    return { "Bond": "James Bond", "Rosenberg": "Willow Rosenberg" }.get(last_name)
    
def find_full_name_v3(last_name: str) -> str:
    return find_full_name_v1(last_name) or (lambda: (_ for _ in ()).throw(ValueError("Full name not found")))()
```
- Coverage limitations
- 100% coverage is expensive and useless

---

# Example 2: Test driven development

- The main idea is to write the tests first
- Then write the code to make them pass
- Refactoring is easy because we have a clear picture of what we want to achieve
- But sometimes writing the tests takes more time than writing the code

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
