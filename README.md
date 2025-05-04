# README Template

Below is a template provided for use when building your README file for students.

# Project Title

Project description goes here.

## Getting Started

Instructions for how to get a copy of the project running on your local machine.

### Dependencies

```
Examples here
```

### Installation

Spacy is used


pip install spacy --> add to requirements.txt
python -m spacy download en_core_web_sm

import spacy
nlp = spacy.load('en_core_web_sm')

Sentiment analysis the following needs to be added:

pip install spacytextblob --> add to requirements.txt
Downloading the respective data
python -m textblob.download_corpora
from spacytextblob.spacytextblob import SpacyTextBlob

Step by step explanation of how to get a dev environment running.

List out the steps

```
Give an example here
```

## Testing

Explain the steps needed to run any automated tests

### Break Down Tests

Explain what each test does and why

```
Examples here
```

## Project Instructions

This section should contain all the student deliverables for this project.

## Built With

* [Item1](www.item1.com) - Description of item
* [Item2](www.item2.com) - Description of item
* [Item3](www.item3.com) - Description of item

Include all items used to build project.

## License

[License](LICENSE.txt)
