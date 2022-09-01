#### jubilant-robot-hacker

# **AI Village Capture the Flag @ DEFCON**

##### Hack AI! Collect flags by evading, poisoning, stealing, and fooling AI/ML

Goal is to help Henry Hacker get to Homecoming during [DEFCON30](https://defcon.org/html/defcon-30/dc-30-index.html), [AI Village](https://aivillage.org/) while interacting with various machine learning security challenges.

### **Process**

In [this](https://www.kaggle.com/competitions/ai-village-ctf/overview) capture-the-flag (CTF), competitors have to interact with API endpoints or code/objects stored in the input directory during each of the challenges. Upon successful completion of a challenge, that challenge will return a flag (unique-to-you strings with a length of 128 characters). To update the scoreboard, competitors will submit a .csv containing all of their flags -- [see the kaggle documentation](https://www.kaggle.com/docs/competitions#submitting-by-uploading-a-file) or contact the competition organizers for help. Cumulative scores will be weighted based on the difficulty of the challenge. All competitors start at 0 and work their way towards a perfect score of 1.0. There are 22 challenges so ensure your submission.csv has exactly those 22 challenge rows.

**NOTE**: The template notebook is just a convenience function and method for submitting flags to the scoreboard but there is no need to feel constrained to that single operating environment. Challenges can be interacted from local host machine that can access the internet after which your flags can be transported into the notebook and scoreboard updated. Kaggle's [competition documentation](https://www.kaggle.com/docs/competitions) includes instructions on submitting predictions.

### **Challenges**

CTF's are inherently puzzles that are intended to challenge you and help you learn new things. Sometimes they may be a little ambiguous or misleading. That's part of the challenge!

- **Math Challenges**: Four challenges to explore the concept of dimensionality.
- **Hotdog and Hotterdog**: Dogs and classifiers. What more could you want?
- **bad2good**: Can you poison a dataset to change how something is classified?
- **baseball**: Can you impersonate someone else by throwing the correct distribution of pitches?
- **crop**: Two challenges to test your ability to manipulate an image cropping model.
- **deepfake**: There's a nasty deepfake getting detected out there, can you help it?
- **honorstudent**: Can you change an image of an F to look like an A? Why would someone want to do such a thing?
- **salt**: This model has some pretty advanced defenses. Can you evade it anyway?
- **theft**: Can you steal this model to get a sneaky owl past it?
- **token**: Sentiment Analysis. Who needs?
- **waf**: A web-app-firewall blocks malicious requests. Can you discover and by-pass the 0-day?
- **inference**: I think something's backwards here. Can you, like, back something out?
- **forensics**: Nice artifact you got there, shame if there was a flag in it.
- **leakage**: Get a password out of a model, is that even possible?
- **murderbot**: Save the humans, escape the bots!
- **secret_sloth**: That sloth has a message. Why? I don't know, but it does.
- **wifi**: Can you pull your wifi password out of the embedding?

### **Data Description**

Dataset can be downloaded using kaggle API ```kaggle competitions download -c ai-village-ctf```.

**NOTE**: Dataset is given in this repository, but you need to add a ```.pckl``` file before starting off. You need to download and place ```04JUN_crop_model.pckl``` file in the ```../ai-village-ctf/crop/``` directory.

This CTF follows a different flow than Most Kaggle Competitions. Competitors will be interacting with API endpoints during each of the challenges. Upon successful completion of a challenge, that challenge will return a flag (a 128 character string). To update the scoreboard, competitors will submit a .csv containing all of their flags. This can be done by uploading a file with all of your flags. There is a [template](https://github.com/anubhavde/jubilant-robot-hacker/blob/main/template.ipynb) for reference purpose. Cumulative scores will be weighted based on the difficulty of the challenge. All competitors start at 0 and work their way towards a perfect score of 1.

### **Files**
- ```sample_submission.csv``` - a sample submission file in the correct format
- Other files are used for specific challenges and referenced in the template notebook.

### **Columns**

- ```challenge_id``` - The challenge id (found in the markdown header)
- ```flag``` - The case-sensitive flag
