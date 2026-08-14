# ⚡ Quick GitHub Pages Tutorial by pxoqxo
I created this quick tutorial for testing GitHub Pages. I always deploy from the `main` branch.

## 🚀 Set Build and Deployment
If you want to stay simple and easy, you need to **deploy from a branch**. If you want full automation, use **GitHub Actions**.

## 🎁 Locations Supported by GitHub Pages?
If you selected "Deploy from a branch", then you need to select your branch first. This means choosing in which branch your pages will live. I simply always select `main`.

Then you need to select the folder location. GitHub Pages supports two folders: `/(root)` and `/docs`.

- **Root folder**: What your repository URL is, your home/root folder. In my case, it's **[0x476974/github-pages](https://github.com/0x476974/github-pages)**.
- **Docs folder**: Simply a folder inside your root.

### 🎈 When to Use Root and Docs Folder?
I really won't comment on official rules, but here's how I personally use them:
- **When you have a main website repository**, i.e., `username.github.io` repository — it won't have any source code in this case. Use **root**.
- **But when you have a project repository having source code**, then use **docs** as documentation and reference for GitHub Pages.

**Short rule**: Use `docs` when you have source code; else if the repository represents a full document, use **root**. 📁

## 🎨 Format Supports
GitHub Pages supports both **Markdown** format and **HTML** format by default. 

- If you have HTML pages, such as `about-us.html`, you can access them directly via `domain.com/about-us.html`. Pretty simple! 😊
- But if you use Markdown (.md) format, such as `about-us.md`, you can access it via `domain.com/about-us.md`, **but this shows raw Markdown data**. Browsers only support HTML format natively. 🤷‍♂️

That's why GitHub Pages uses **Jekyll** to convert Markdown to static sites. Once you publish the site, GitHub Pages automatically converts `.md` files to `.html`. So if you have `about-us.md` and want to use it as HTML, simply use `domain.com/about-us.html`, **not** `domain.com/about-us.md`. 

- **Markdown (.md)** files will show you raw data written by you in your browser. 📝
- **HTML (.html)** files will show you automatically converted HTML files. ✨

You can make templates and other designs using Jekyll, but I'm not talking about that here.

### 🎈 Format Benefits
Personally, I am using **Markdown files only** since they are flexible in my repository and in my website too. Also, Markdown format can have HTML code, but HTML files don't support Markdown. 

If you want some custom page layout, use **HTML**. So you can have some `.html` files and some `.md` files with a **mixed approach**. 🔄

This mixed approach is cool when you need custom design over documentation. 👌

### ⚠ Naming Warning
Remember: if you have the same-named `.md` and `.html` files in the same folder, i.e., `about-us.html` and `about-us.md`, then the `.md` file will **not** convert to HTML format and the direct `.html` file will be accessed. **Avoid naming conflicts!** 🚫

## 🔗 Default Home Page
Page names are **case-sensitive**, so be careful while browsing URLs in your browser. First, I will show you all results clearly. I'll keep it minimal to show which are working and which are not. ✅❌

I tested with `Default`, `Home`, `Index`, and `Readme` — all 4 names. The combinations are `.md` and `.html` formats, plus uppercase, lowercase, and camelCase as case styles. **So 4 Names × 2 Formats × 3 Case Styles = 24 Combinations!** 🧮

And trust me, below filenames browsers can take as default page:
- `index.html` ✅
- `README.md` ✅
- `index.md` ✅
- `readme.md` ✅
- `Readme.md` ✅

And below filenames GitHub can take as default page. Keep in mind: all HTML files supported in GitHub Preview show raw data unlike Markdown rendering:
- `README.html` ✅
- `readme.html` ✅
- `Readme.html` ✅
- `README.md` ✅
- `readme.md` ✅
- `Readme.md` ✅

### 🎈 So What to Prefer?
Personally, I told myself: **I will use only Markdown files**, so `README.md` is best. For any custom page, name it like `how-to-do-stuff.md`. 📄

## ❌ Location Conflicts and Default Priority
Let's assume there's a `USERNAME.github.io/Example1` folder available, and also a same-named `Example1` repository which also has GitHub Pages enabled. **This is what I call a conflict!** 💥

In GitHub, I tested and got this result: GitHub Pages gives **priority to the repository**, and the `Example1` directory will be **inaccessible**. 

Keep this in mind and **avoid such conflicts**! 🔒

## 🏁 Remark
OK, so everything in this blog about GitHub Pages is covered here. If I remember something I missed or need to add something new, I will update it later! 📅✨