# End-to-End CI/CD Pipeline for Node.js Web Application using AWS CI/CD Services 🚀

Build a CI/CD pipeline for a Node.js web application using AWS CI/CD services (**CodeBuild, CodeDeploy, CodePipeline**).

## Architecture Description 📝

Here's a quick look at the CI/CD pipeline architecture:

**1. Commit to GitHub:** When users push a new commit to the GitHub repository, it triggers the pipeline. 

**2. Pipeline Stages:** 

- **Source:** Pulls the source code from the GitHub repository.
- **Build:** Uses AWS CodeBuild to test the Node.js web application.
- **Deploy:** Uses AWS CodeDeploy to deploy the Node.js web application to an Elastic Beanstalk environment.

**Note:** In this project, the build stage is used to test the Node.js web application. In a real-world scenario, you would also include the build process in this stage.

## Architecture Diagram 📌
![diagram](https://github.com/user-attachments/assets/c5919c0d-8e00-4c74-a22a-79058b45c67d)

## Prerequisites 📋

- An AWS account with the necessary permissions to create the required resources.
- GitHub account

## Steps 📝

| Step No | Document Link |
| ------ | ------ |
| 1 | [Create a Instance role Elastic Beanstalk][Step-1] |
| 2 | [Configure Elastic Beanstalk Environment][Step-2] |
| 3 | [Create a Pipeline to Deploy Node.js Application][Step-3] |
| 4 | [View the Application][Step-4] |
| 5 | [Clean Up][Step-5] |


   [Step-1]: <./Steps/step1.md>
   [Step-2]: <./Steps/step2.md>   
   [Step-3]: <./Steps/step3.md>
   [Step-4]: <./Steps/step4.md>
   [Step-5]: <./Steps/step5.md>

## Usage 🛠️

1. Clone or download the repository.
```sh
git clone https://github.com/Daoud-Hussain/AWS-CICD-Node-App
```
2. Follow the steps mentioned in the [Steps](#steps-) section.
3. Clean up the resources by following the [Clean Up](./Steps/step5.md) steps.

## Contributing 🖇️

Pull requests are welcome for any changes.

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Author 🙋‍♂

- [Daoud Hussain](https://www.linkedin.com/in/daoud-hussain/) on LinkedIn.
- You Can also check out my [Medium](https://medium.com/@dev.daoudhussain) for articles on DevOps Tools and Technologies.️
