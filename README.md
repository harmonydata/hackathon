# Harmony is planning a hackathon!

* [FAQs here](./FAQs.md)
* [Judging criteria (mark scheme)](./judging-criteria.md)

We are planning a hackathon in London on 3 June. [You can sign up on Eventbrite](https://www.eventbrite.com/e/harmony-hackathon-tickets-887795278577)!

In the meantime, feel free to join our [community](https://harmonydata.ac.uk/community) on Discord, check out the [ideas list](/ideas) and try our [Kaggle competition](https://harmonydata.ac.uk//kaggle)!

[Sign up on Eventbrite](https://www.eventbrite.com/e/harmony-hackathon-tickets-887795278577)

* When: 3 June 2024, registration starts at 9:00 am
* Where: University College London, Room B02 in [Chandler House](https://www.ucl.ac.uk/pals/contact/how-find-chandler-house), 2 Wakefield St, London WC1N 1PF

The hackathon is for improving Harmony in general and we would like help with a number of areas - your team could pick one or choose your own!

* [Task 1: PDF parsing](./1-pdf-parsing.md)
* [Task 2: Improve matching of items by semantic similarity](./2-matching.md)
* [Task 3: Experimenting with LLMs](./3-add-llms.md)
* [Task 4: adapting Harmony to other domains such as medical history or Informed Consent Forms](./4-other-domains.md)
* [Task 5: Making Harmony multilingual](./5-multilingual.md)
* [Task 6: Getting Likert scales out of documents](./6-likert.md)
* [Task 7: Making a similarity score between instruments using the Word Movers Distance algorithm](./7-similarity.md)
* Plus any ideas you might have! We have some UX issues that could be fixed - see [UX testing report](./UX%20Notes%20on%20Harmony%20Tool.pdf).

Ideas of the problems that we will be solving are here: https://harmonydata.ac.uk/ideas 


# Installing Harmony

You can use Windows, Linux or Mac. We have made some videos to help you install Python and Harmony:

🎬[Video for Windows](https://www.youtube.com/watch?v=Okk8tUMDr6g) · 🎬 [Video for Linux/Mac](https://www.youtube.com/watch?v=enWh0-4I0Sg) · 🎬 [Video on how to install the front end locally](https://youtu.be/1xp3Uh6dptg)

Here are the steps to get started:

* First clone the repository from Git. If you're not familiar with Git and Github, we recommend you watch a tutorial on Git first (example: https://www.youtube.com/watch?v=USjZcfj8yxE)
* Install Python 3.11
* Install Pycharm
* Install Jupyter Notebooks
* Run the [example Colab notebook](https://colab.research.google.com/github/harmonydata/harmony/blob/main/Harmony_example_walkthrough.ipynb)

* We recommend Anaconda and Jupyter Notebook
* Then you can do `pip install harmonydata` to install Harmony once Python has been installed.

# Pushes and commits

We try to keep our code clean and consistent. If one person uses spaces and another uses tabs, it's hard to manage it and keep track of code changes. Please follow the general principles for consistency.

When developing and pushing changes,

* Please use [PEP-8 Linter](https://pypi.org/project/pep8/) - this is a set of rules of how many whitespace characters are allowed in a line, and in general provides consistency for formatting of human readable code and comments. If everyone formats their code differently, things become hard to manage as it's hard to track if a change is a functional change, or a formatting change. Imagine if a newspaper article switched between British and American spelling every sentence and between formal tone and textspeak! Let's keep things consistent!
* Please run unit tests before pushing. We use test driven development. That means that every commit gets tested automatically by Github and will get a green tick or red cross if the tests pass or fail. All the repos have tests in a folder called `tests` and you can run them on your computer and Github actions will run them when you commit. They will tell you if you break any functionality.
* Check your PR hasn’t got any extra files made by your IDE that shouldn’t be committed, such as .vscode. It's a common mistake for beginners to bulk commit the entire contents of a directory including files which are not part of the project. For example, Mac puts extra hidden files inside folders when you open them in the file browser. Try not to let them clutter our code base. They make code hard to manage and in some cases can break the tool.

# At the end of the hackathon

Please fill out our feedback form at the end of the session: https://forms.gle/WSXaoDiWu7XF8oKr5
