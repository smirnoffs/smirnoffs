## Quality Engineering

I'm a big fan of a quality engineering approach in which developers design, build and maintain their own quiality pipeline. Every aspect of the quality assurance that can be automated should be automated. 
<details>
    <summary>Ideal CI/CD pipeline</summary>
High level of automation allows to eleminate unnecessary controls (manual QA, code reviews, manager's approval). And all the automation should be a part of your CI/CD.
  
The ideal pipeline:
  - Static code analyzers, linters, format checks - this part is the simplest and automate most of things that we see in code review comments, there is no need to leave comments about the code style, automate it!
  - Unit tests
  - Docker build 
  - Deploy to the Staging or any stage that is not production and close to your Production. I worked in companies where services were deployed into multiple stages, such as QA, dev etc. In most cases you need just Staging and Production.
  - behavioural tests against your Staging - here you need to make sure that the service behaves in the way you need and the behaviour doesn't change. In python I use [behave](https://behave.readthedocs.io/en/stable/) in Go I use [Ginkgo](https://github.com/onsi/ginkgo).
  - Deploy to Production
  - Tests on production - yes, tests on production. You need to check if you production works OK, the easiest way is to do it with a subset of your behaviour tests. 
</details>


## My favorite books, blogs, podcasts

### Science-fiction
Before 2006 I thought that science fiction is dead. But then [Blindsight](https://en.wikipedia.org/wiki/Blindsight_(Watts_novel)) by Peter Watts was published, and I read it 4 times in a row. Watts set the bar extremely high. [Seveneves](https://en.wikipedia.org/wiki/Seveneves) by Neal Stephenson IMO is one of the best science fiction book of last years.

### Tech
- [Accelerate: The Science of Devops](https://www.amazon.de/-/en/Nicole-Ph-D-Forsgren/dp/1942788339/) - must-read for every engineer and manager. The current development process in our team is heavily influenced by this book.

### Podcasts
- [Lex Fridman podcast](https://lexfridman.com/podcast/) helps me to be open-minded and accept different points of views. Lex is brilliant AI Researcher and he speaks with scientists, engineers, sportsmen, writers who literally shape this world.
- [The Changelog](https://changelog.com/podcast) podcast is my source of fresh ideas and news from the world of technologies.
- [Радио-Т](https://radio-t.com) - russian-speaking podcase that I listen since 2006. I must say that quite some of my life decisions were made by the influence of podcast's hosts: buying first Mac, learning Java, Python, Go, focusing on the backend, endless decisions about the infrastructure and libraries. 
