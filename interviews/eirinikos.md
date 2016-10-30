
## Andrea Kao, Homebrew 🍻

**What's your story in a few sentences?**
I grew up in Simi Valley, went to college in the Bay Area, and have been back in southern California for the past 10 years. I got interested in programming a few years ago, when I learned about physical computing (i.e., the amazing stuff that's done with Arduino, Raspberry Pi, etc.). Ironically, none of the work I’ve actually done involves physical computing!

**How did you hear about Outreachy? What made you want to apply?**
I heard about Outreachy in a Women Who Code weekly newsletter. It was less than 2 weeks until the application deadline and I had serious doubts about my ability to contribute to Homebrew, but the project mentor was very encouraging. Plus, Homebrew was the only summer Outreachy project that involved things I knew how to use (Ruby, Git, GitHub, and OS X).

**What was the application/interview process like?**
The entire program and its processes are documented on a [Wiki page](https://wiki.gnome.org). After I learned about Outreachy and Homebrew’s participation, I read the info on Homebrew’s [Summer of Code repo](https://github.com/Homebrew/Outreachy-and-Google-Summer-of-Code) and then emailed the mentor to introduce myself. He gave me some pointers on how to make my first contributions and answered all my questions. I spent the next two months reading as much Homebrew code and documentation as I could (even though I couldn't understand it all) and submitting small contributions for various [core formula](https://github.com/Homebrew/homebrew-core) files.

There’s only an application to submit for Outreachy (no interview). You’re required to make at least one contribution to the project before submitting your application, and you’re encouraged (urged) to make more contributions throughout the application period. You can make changes to the application throughout this time (i.e., you can update a running list of contributions).

**What was your first commit/fix/issue for Homebrew?**
My first [pull request](https://github.com/Homebrew/homebrew/pull/50151) was a small fix for [gf-complete’s](http://jerasure.org/) formula file. I removed a line that redundantly stated the version number for gf-complete.

**Talk about the tools you use. What language do you write? In what app?**
I write Ruby in Sublime Text using the [Rubocop linter](https://github.com/SublimeLinter/SublimeLinter-rubocop) to catch style violations; in Sublime, I display a ruler at 80 characters to catch lines that are too long.

![sublime]({{site.github.url}}/images/2016-08/sublime.png)

To familiarize myself with how **`brew`** commands work, I run them in the shell, I look them up in the man pages, and I read their code; I also use **`brew irb`** to play with methods written in Homebrew's DSL, particularly ones from the [Formula](http://www.rubydoc.info/github/Homebrew/brew/master/Formula) API.

![brew irb]({{site.github.url}}/images/2016-08/brew_irb.png)

[Rubular](http://rubular.com/) is helpful (to play with regexes).

![rubular]({{site.github.url}}/images/2016-08/rubular.png)

And I keep several browser tabs open and pinned for reference:

- [SimpleCov](https://github.com/colszowka/simplecov) reports (for the entire test suite as well as for the test(s) that I’m working with)
- [Homebrew's API](http://www.rubydoc.info/github/Homebrew/brew/master)
- [Homebrew's Formula Cookbook](https://github.com/Homebrew/brew/blob/master/share/doc/homebrew/Formula-Cookbook.md)
- [Homebrew's How to Open a PR (and get it merged)](https://github.com/Homebrew/brew/blob/master/share/doc/homebrew/How-To-Open-a-Homebrew-Pull-Request-(and-get-it-merged).md)

**How do you talk to your coworkers/colleagues?**
We (the Google Summer of Code and Outreachy interns) have a **#gsoc-outreachy** channel for open group discussion within Homebrew's Slack group. We use direct messages, too.

**What do you use GitHub.com for?**
All of Homebrew’s repositories are hosted on Github. I reference Homebrew’s [share docs](https://github.com/Homebrew/brew/tree/master/share/doc/homebrew) (stored in the [**`Homebrew/brew`** GitHub repo](https://github.com/Homebrew/brew)) and I submit [pull requests](https://github.com/Homebrew/brew/pulls) for my work. And updating Homebrew itself is effectively the same as pulling updates from its remote master repo into your local repo.

**What do you do if you have a question?**

- Google it to death
- check Ruby Docs and [Homebrew’s extended modules & classes](https://github.com/Homebrew/brew/blob/master/Library/Homebrew/extend/)
- check Homebrew’s [Formula](http://www.rubydoc.info/github/Homebrew/brew/master/Formula) API
- ask a maintainer (via GitHub or Slack)

**More screenshots!...**

My main task this summer has been to increase Homebrew's test coverage. Running **`brew tests`** tells **`rake`** to run all of the unit and integration tests that live inside the **`Homebrew/test`** directory. Adding the **`--coverage`** option tells SimpleCov to generate an HTML report that you can view in your browser.

![brew tests]({{site.github.url}}/images/2016-08/brew_tests.png)

Here's a recent SimpleCov report! (It lives at **`Homebrew/test/coverage/index.html`**.) Almost all of my work has involved testing **`brew commands`**, so the **`Homebrew/cmd`** files are what I'm particularly concerned with.

![simplecov]({{site.github.url}}/images/2016-08/simplecov.png)

And here's the checklist you're asked to complete before you submit a pull request to the **`Homebrew/brew`** repo:

![pr checklist]({{site.github.url}}/images/2016-08/pr_checklist.png)
