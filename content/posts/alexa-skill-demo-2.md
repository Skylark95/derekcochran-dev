+++ 
draft = false
date = 2022-03-26T00:07:24-05:00
title = "Alexa Skill Demo (Week 2)"
description = "Alexa Skill Demo for Normal Community High School State Farm STEM Program"
tags = ["Java", "Lambda", "AWS"]
categories = ["STEM", "Alexa"]
series = ["alexa-skill-demo"]
+++

# Alexa Skill Demo

To view the steps from last session click [here](https://github.com/Skylark95/alexa-skill-demo/blob/2022-03-18/README.md)

## Add an Alexa Skills Kit trigger
1. Log in to the AWS Management Console and navigate to AWS Lambda\
![lambda](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/lambda.png)

2. Click your function in the list to open the configuration details

3. Click **Add Trigger**\
![add trigger](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/add-trigger.png)

3. Under add triggers, click **Alexa Skills Kit** to select the trigger.\
![add trigger](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/add-trigger-2.png)

4. Under Configure triggers, select Enable for Skill ID verification.

5. Make sure Skill ID verification is Enabled.

6. Enter your Skill ID in the Skill ID edit box.

7. Click **Add**.
![alexa skills kit trigger](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/alexa-skills-kit.png)

8. Go to the **Function ARN** Google Sheet and enter **yes** next to your group under the **Skill ID Added to Lambda**.

## Clone Repository
9. Open Visual Studio Code click the **Source Control** Button.\
![source control button](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/source_control.png)

10. Click Clone repository. In the text prompt provide the url: https://github.com/Skylark95/alexa-skill-demo.git\
![clone repository](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/clone_repository.png)

## Edit the Skill Code
11. Click the **Explorer** Button.\
![explorer](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/explorer.png)

12. Expand the **src** and **handlers** directory and open `HelloWorldIntentHandler.java`\
![hello world](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/hello-world.png)

13. Edit the `speechText` in the `handle` method to say something unique for your group. Get creative. Don't just keep the standard `"Hello World"`, this will be what makes your skill unique for your group. Be sure to save the file when you are done.

## Build The Skill Code
13. Open the Visual Studio Code _Command Pallete_ (`Ctrl` + `Shift` + `P`) and select _Tasks: Run Build Task_ to build a jar file for your skill. The jar file will be output to the project directory with the name _alexa-skill-demo.jar_\
![run build task](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/run_build_task.png)

## Upload the Jar File to your Function
16. Upload the JAR file produced in the previous step under Function code.\
![upload jar](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/upload_jar.png)

17. Your code is now deployed. See a mentor and let's run your new Alexa Skill!

## Bonus
There is much more you can do. Below is a link to Amazon's documentation on Alexa skills. Check it out and see what else you can do!

## Resources
- https://developer.amazon.com/en-US/docs/alexa/alexa-skills-kit-sdk-for-java/develop-your-first-skill.html