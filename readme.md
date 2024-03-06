# rocket-tech-gsu.github.io

## Contributing
If you want to make changes to the website, here's how:

### Step 1: Forking the central repository.
- We host the central repository for the website at https://github.com/rocket-tech-gsu/rocket-tech-gsu.github.io
- All of the website code is stored in the `gh-pages` branch, not in the `main` branch!
- You'll need to fork that repository: Go here https://github.com/rocket-tech-gsu/rocket-tech-gsu.github.io/fork and **_uncheck the checkbox that says "Copy the main branch only_"**.
- Then you should be taken to your fork.

### Step 2: Switching branch and starting a Codespace.
- Click on the `main` button on the left side, then click on the `gh-pages` branch to check that branch out (this is where all the website source code is stored).
- Click on the green `Code` button on the right side, then click the `+` button to create a new Codespace.
- You should be taken into the codespace. You should see a terminal at the bottom. If not, click the three horizontal lines at the very top left of the Codespace page, click Terminal, then New Terminal.
- Type `git checkout gh-pages` into the terminal (just to be sure) and press enter.
- Type `gem install jekyll bundler` into the terminal and press enter.
- Type `bundle add webrick` into the terminal and press enter.
- Type `bundle exec jekyll serve` into the terminal and press enter.
- You should see a little dialog box pop up at the bottom right after a couple of seconds. Click the blue Open in Browser button on it.
- Now you should be taken to a development server running the website locally on your Codespace! You can edit the website content now and Jekyll will automatically update the site so you'll see it as soon as you reload the webpage.

### Step 3:  How to edit the website.
- Want to edit the website theme/layout? Google "Jekyll GitHub Pages theme edit" and look around for basic info -- this is a little more involved anyway, so I won't describe it here.
- Want to create a blog post? Copy an existing one (a `*.markdown` file) in `_posts` and edit the date and title in the filename as you wish, then change the file contents however you like.
- Want to edit a non-blog-post webpage? Edit one of the `*.markdown` files in the top-level directory (for instance, `index.markdown` or `about.markdown`).
- Want to create a non-blog-post webpage? Copy one of the `*.markdown` files in the top-level directory and change its name and contents however you like.
- Want to host some content (photos, video, files, etc.) on the website? Stick it in the `assets` directory. You can nest folders in `assets` to help you keep things organized. It's a good idea to make a separate folder for each page or blog post. You can then reference files in `assets` from the markdown you write in blog posts and webpages.

### Step 4: Pushing the changes.
- Commit and push any changes you make back up to your GitHub repository when you're satisfied.
- Make a pull request when you're ready to contribute code to the production version of the website.
- Ping either @Varun (President) or @Carter (Advisor & Mentor) to review the pull request if we're taking more than an hour or two. (Don't spam us repeatedly though, please.)
- A GitHub Actions workflow will run once we merge the pull request, and within a few minutes you should see the changes go live.

## Website Layout:
1. About Page(also, it should be the landing page):
  - Team section (with their LinkedIn)
  - Board section (with their emails n LinkedIn)
2. Sponsors page:
  - "Be our sponsor" section
  - Current Sponsors
  - Past Sponsors
3. Learnings Page:
  - Physics Sub-Page
  - Softwares Sub-Page
  - Avionics Sub-Page
  - Design Sub-Page
  - Manufacturing Sub-Page
