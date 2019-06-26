## Alexa-APL-Fact-Skill - Monkey Facts

Welcome!  You too create a "Fact Skill Compatible with APL" with the help of the Monkey Facts skill!  OK, just kidding, maybe.  This sample skill  demonstrate the Alexa Presentation Language (APL).  Ask for a fact and you'll be provided with an image and a fact about Monkey.

## Prerequisites

* An Alexa Developer Account (sign up here: https://developer.amazon.com/alexa-skills-kit)
* (Optional) An AWS Account (sign up here: https://aws.amazon.com)
* (Optional) An Amazon Echo Device with a screen (e.g. Amazon Echo Show)

> Note: The AWS Account is optional because you can create this sample as an Alexa Hosted skill.  The Echo Show is optional because you can see the display in the simulator.

## Brief Steps

> Note: The below steps assume you have general familiarity with how to use the Alexa Developer Console.  If you've never created a skill before, check out the [fact skill](https://github.com/alexa/skill-sample-nodejs-fact) tutorial to get the feel for it.


1. From the [Alexa Developer Console](https://developer.amazon.com/alexa-skills-kit) create a new skill.
    1. Name the skill whatever you want, but we recommend `Monkey Facts`!
    1. Choose the language model you want to use, as long as as it is `English (IN)` which corresponds to **en-IN**.  The skill is ready for other Locale too.
    1. Choose the **Custom** interaction model.
    1. Choose **Alexa Hosted**.
1. It may take a minute, but when your skill is ready, go to the **JSON Editor** section and replace all the contents with the interaction model from [here](https://github.com/rimmi21/Alexa-APL-Fact-Skill/blob/master/json-editor.json) .  Click **Save Model**.
1. Click on **Interfaces** and enable **Alexa Presentation Language**.  (**Auto Delegation** should already be enabled.)
1. Save that change and build your model.
1. Click on the **Code** tab and update the following files with the contents from this repo:
    * **index.js** with this [index.js](./lambda/index.js) (Pro tip: click the **Raw** button to make it easier to copy)
    * **package.json** with this [package.json](./lambda/package.json)

1. In the **lambda** folder, create a file named `main.json`  and source the contents from [here](./json-editor.json).

1. Save and Deploy the function
1. Click on the **Test** tab, enable the skill and check it out.  Phrases you can try include:
    * `open monkey facts` (or whatever invocation name you used)
    


