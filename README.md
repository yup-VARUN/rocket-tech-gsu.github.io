# rocket-tech-gsu.github.io
Rocket Tech GSU's official website

---

# Contributing
If you want to make changes to the website, here's how:

## Step 1: Forking the central repository.
- We host the central repository for the website at https://github.com/rocket-tech-gsu/rocket-tech-gsu.github.io
- All of the website code is stored in the `gh-pages` branch, not in the `main` branch!
- You'll need to fork that repository: Go here https://github.com/rocket-tech-gsu/rocket-tech-gsu.github.io/fork ***and uncheck the checkbox that says "Copy the `main` branch only".***
- Then you should be taken to your fork.

## Step 2: Switching branch and starting a Codespace.
- Click on the `main` button on the left side, then click on the `gh-pages` branch to check that branch out (this is where all the website source code is stored).
- Click on the green `Code` button on the right side, then click the `+` button to create a new Codespace.
- You should be taken into the codespace. You should see a terminal at the bottom. If not, click the three horizontal lines at the very top left of the Codespace page, click `Terminal`, then `New Terminal`.
- Type `git checkout gh-pages` into the terminal (just to be sure) and press enter.
- Type `gem install jekyll bundler` into the terminal and press enter.
- Type `bundle add webrick` into the terminal and press enter.
- Type `bundle exec jekyll serve` into the terminal and press enter.
- You should see a little dialog box pop up at the bottom right after a couple of seconds. Click the blue `Open in Browser` button on it.
- Now you should be taken to a development server running the website locally on your Codespace! You can edit the website content now and Jekyll will automatically update the site so you'll see it as soon as you reload the webpage.
