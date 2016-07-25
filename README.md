# LazierTesting

This was forked to adapt to our team's lazier/agiler workflow.

A node.js based program for parsing manual gherkin/cucumber feature files and generating a pdf based manual test plan.

### Requirements
node: https://nodejs.org/en/download/

npm (Usually bundled with node)

### Running

<b>NOTE:</b> Programs such as Skype must not be occupying your port before running.

First create a configuration file `config.json` based off the following template in the directory that contains `lazy.js`. 
```
{
  "port": 6969,
  "featureFilesFolder": "C:\\Path\\To\\Manual\\Feature\\Folder",
  "names": [
    "Your name"
  ],
  "testingTags": [
    "manual"
  ]
}
```

Then run these commands in the root of the project:
```
npm install
node lazy.js
```
Then navigate to `localhost:<portNumber>` in a web browser.

Feature files must have the `@manual` annotation as the first line in order for them to show up.

Click `Auto-assign` to assign all of the tasks to yourself.

Once you have completed all of the tests, save the resulting PDF locally. All the PDF's will be aggregated at an appropriate time.

### Credit
The lovely SENG302 students who showed this to us, thanks a bunch!

### License
MIT License on all original code. All other code is under it own respective licenses.
