# draft-recognizer

This respository contains the files for the webapp I've hosted on
https://draft-recognizer.herokuapp.com/. The app classifies an image as part of
the draft phase or not part of the draft phase in the game
[Pirates Outlaws](https://fabledgame.com/en/pirates-outlaws/details). The draft
phase is the part of the game where the player chooses from a random selection
of cards or relics.

![draft recognizer](https://user-images.githubusercontent.com/46179386/125207332-8a3d7580-e240-11eb-8f02-37b75298b863.gif)

---

### Table of Contents

- [draft-recognizer](#draft-recognizer)
    - [Table of Contents](#table-of-contents)
- [Note](#note)
- [Introduction](#introduction)
- [Use](#use)

# Note

The heroku app may take about a minute to load. In the mean time, you can search
for a link to a Pirates Outlaws image on Google.

# Introduction

<a href="https://fabledgame.com/en/pirates-outlaws/details" alt="Link to Pirates Outlaws.">Pirates
Outlaws</a> is a card game by Fabled Game Studio. In this web app, I created a
classifier using fast.ai, Heroku, and Python that classifies whether or not the
image was taking during the game's draft phase, where you select a card to place
into your deck. The data I used to train this model consists of frames that I
pulled with ffmpeg from my own recorded video.

# Use

Open https://draft-recognizer.herokuapp.com/ to start loading and then find a
link to a screenshot of Pirates Outlaws to classify. Once the Heroku app loads,
you can click `webapp.ipynb` if it's on the screen. You can paste your link into
the field and then do these clicks: `Upload Link`, `Classify`, `Refresh Image`.
`Refresh Image` will show the image you're currently classifying. By default, an
image of the draft phase is loaded if the link supplied is not valid.
