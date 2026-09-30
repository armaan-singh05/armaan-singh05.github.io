# Armaan Singh — Portfolio

My personal engineering portfolio, hosted free on GitHub Pages at
**https://armaan-singh05.github.io**

You can make every edit below right on github.com: open a file, click the ✏️ pencil icon,
change it, then click **Commit changes**. The site updates about a minute later.

---

## Where things live

| What you want to change | File |
|---|---|
| Bio, contact links, skills, experience, education, awards | `_data/profile.yml` |
| Projects (one file per project) | `_projects/` |
| Project pictures | `assets/img/projects/<project-name>/` |
| Resume PDF | `assets/Armaan_Singh_Resume.pdf` (upload a new file with the same name) |
| Colours and fonts | `assets/css/style.css` (the colour values at the top) |
| Page layout (you usually won't need this) | `index.html`, `_layouts/` |

---

## Add a new project

1. **Upload pictures (optional).** On your computer, put the pictures in a folder named after
   the project (e.g. `my-robot`). On GitHub, open `assets/img/projects/`, click
   **Add file → Upload files**, and drag the whole folder in. The pictures end up at
   `assets/img/projects/my-robot/cover.jpg` and so on.
2. **Create the project file.** Open `_projects/_TEMPLATE.md`, copy everything, then go to
   `_projects/`, click **Add file → Create new file**, name it something like `my-robot.md`
   (lowercase, no spaces), paste, and fill it in.
3. **Commit.** The project appears on the home page automatically, sorted newest first by
   `date`, and gets its own page at `/projects/my-robot/`.

A project file looks like this. Only `layout`, `title`, `date` and `summary` are required:

```markdown
---
layout: project
title: My Robot
course: ENSC 000                                  # optional
date: 2026-10-01                                  # sorts projects, shows as "Oct 2026"
summary: One or two sentences for the home page card.
tags: [C++, PCB Design]
image: /assets/img/projects/my-robot/cover.jpg    # optional cover picture
links:                                            # optional buttons
  - label: GitHub
    url: https://github.com/armaan-singh05/my-robot
gallery:                                          # optional picture grid
  - src: /assets/img/projects/my-robot/build.jpg
    caption: The finished build
---

## Overview

Write about the project here, in normal Markdown.

![A picture in the middle of the text](/assets/img/projects/my-robot/diagram.png)
```

Projects without an `image` get a clean placeholder card that shows the course code.

**Picture tips:** use `.jpg` for photos and `.png` for diagrams and screenshots. Keep each file
under about 1 MB (resize large phone photos first). Cover images look best in landscape (16:9).
File names are case-sensitive, so `Cover.JPG` and `cover.jpg` are different files.

**Hide or remove a project:** delete its file, or add `published: false` to its front matter.

---

## Preview locally (optional)

```bash
gem install jekyll
jekyll serve        # then open http://localhost:4000
```

## GitHub Pages setting

In the repo, go to **Settings → Pages** and make sure **Source** is set to
*Deploy from a branch*, using the `main` branch and the `/ (root)` folder.
