# Harmony is planning a hackathon!

We are planning a hackathon in London on 3 June. Sign up and we will contact you with the details!

In the meantime, feel free to join our [community](https://harmonydata.ac.uk/community) on Discord, check out the [ideas list](/ideas) and try our [Kaggle competition](https://harmonydata.ac.uk//kaggle)!

Sign up link is coming up on Eventbrite soon!

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

* Please use PEP-8 Linter
* Please run unit tests before pushing. We use test driven development. That means that every commit gets tested automatically by Github and will get a green tick or red cross if the tests pass or fail.
* Check your PR hasn’t got any extra files made by your IDE that shouldn’t be committed, such as .vscode

# At the end of the hackathon

Please fill out our feedback form at the end of the session: https://forms.gle/WSXaoDiWu7XF8oKr5
