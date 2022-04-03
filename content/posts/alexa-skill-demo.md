+++ 
draft = false
date = 2022-03-18T12:00:00-05:00
title = "Alexa Skill Demo (Week 1)"
description = "Alexa Skill Demo for Normal Community High School State Farm STEM Program"
tags = ["Java", "Lambda", "AWS"]
categories = ["STEM", "Alexa"]
series = ["Alexa Skill Demo"]
+++
This is part of a the Alexa Skill Demo series for Normal Community High School State Farm STEM Program.
To view the steps in the next session click [here]({{< relref "alexa-skill-demo-2.md" >}}).

## Creating The Skill Function in AWS Lambda
1. Log in to the AWS Management Console and navigate to AWS Lambda by searching for it in the search bar.\
![lambda](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/lambda.png)

2. Click **Create function.**\
![create function](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/create_function.png)

3. Make sure to confirm that "Author from scratch" option is selected.\
![author from scratch](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/author_from_scratch.png)

4. Enter a **Function Name** for the function.
5. Select **Java 11 (Correto)** as the **Runtime**
6. Select **x86_64** as the **Architecture**\
![function page](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/function_page.png)

7. Click on **Change default execution role** and select **Use an existing role**. In the Existing Role dropdown select **LabRole**\
![select role](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/select_role.png)

8. Click **Create function.**

9. Copy the **Function ARN** of your AWS Lambda and save it in a location mentioned during the class period.\
![copy arn](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/copy_arn.png)

10. Under **Runtime Settings** on the function page click **Edit**\
![edit runtime](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/edit_runtime.png)
11. Fill in the Handler information with fully qualified class name of your stream handler class (in our example this value will be `com.amazon.ask.helloworld.HelloWorldStreamHandler`)\
![runtime settings](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/runtime_settings.png)

## Clone Repository
12. Open Visual Studio Code click the **Source Control** Button.\
![source control button](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/source_control.png)

13. Click Clone repository. In the text prompt provide the url: https://github.com/Skylark95/alexa-skill-demo.git\
![clone repository](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/clone_repository.png)

## Build The Skill Code
14. Open the Visual Studio Code _Command Pallete_ (`Ctrl` + `Shift` + `P`) and select _Tasks: Run Build Task_ to build a jar file for your skill. The jar file will be output to the project directory with the name _alexa-skill-demo.jar_\
![run build task](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/run_build_task.png)

## Upload the Jar File to your Function
15. Upload the JAR file produced in the previous step under Function code.\
![upload jar](https://raw.githubusercontent.com/Skylark95/alexa-skill-demo/main/img/upload_jar.png)

16. Congratulations! You're done for this session!

## Resources
- https://developer.amazon.com/en-US/docs/alexa/alexa-skills-kit-sdk-for-java/develop-your-first-skill.html