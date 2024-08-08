## Create a Pipeline to Deploy Node.js Application

In this step, we'll set up a pipeline to automatically deploy your Node.js web application to an Elastic Beanstalk environment. We'll use AWS CodePipeline to make the whole deployment process smooth and automated.

### Steps to Create a Pipeline to Deploy Node.js Application:

- Click on Services → All Services → Developer Tools.
- Navigate to CodePipeline.

![17](https://github.com/user-attachments/assets/f7aaec02-39b8-479f-8234-b3d1b4ba4fd7)

-  Click on Create Pipeline.

![18](https://github.com/user-attachments/assets/b93734a3-71f0-481b-a6a9-b6ac3dac7727)
![19](https://github.com/user-attachments/assets/75179605-bd3a-4ee6-9fa3-a33b95bed651)
![20](https://github.com/user-attachments/assets/6a8d893b-d1a7-4595-b278-12c3878da3b8)
![21](https://github.com/user-attachments/assets/414c1fca-6928-4804-adcc-d788568f5d33)

- Connect to Github.
  
![22](https://github.com/user-attachments/assets/c1c091f7-b643-44ef-8719-0a7c9b52a422)
![23](https://github.com/user-attachments/assets/50c20bef-9d99-47a2-bd0b-6bc1524261b0)

- Choose the repository containing your Application code.
  
![25](https://github.com/user-attachments/assets/c712f7b7-6f3c-45b9-b20b-f142fa9de34c)
![26](https://github.com/user-attachments/assets/7423a3a4-3705-4d12-a989-68093cfe5651)
![27](https://github.com/user-attachments/assets/937183e9-4d00-4a6f-a174-d55dc299ef1c)

![28](https://github.com/user-attachments/assets/3bda2860-1ad3-4ec5-8a44-629c024dd884)

- Now, Create Project to add build.

![29](https://github.com/user-attachments/assets/17a4eed5-9321-41b9-ac00-6a95fe590908)
![30](https://github.com/user-attachments/assets/9c644341-fae7-46d7-8705-5120fae8c441)
![30 5](https://github.com/user-attachments/assets/c7ccb36e-ed74-4797-a399-e04d50714e21)
![31](https://github.com/user-attachments/assets/6c78de91-6182-4aff-9be3-adb9cf58d1b5)
![33](https://github.com/user-attachments/assets/76ed0539-292a-4e02-99b0-e6f56b54ae99)

- After build stage is completed, add Deploy Stage.

![34](https://github.com/user-attachments/assets/0c748b21-55f9-4cb5-b5b1-755551f06423)
![35](https://github.com/user-attachments/assets/e6fd44fd-adf6-4c25-ab49-9a8b1c2a43a8)
![36](https://github.com/user-attachments/assets/6944af37-e7e4-4cbc-94a7-ab1a3ddb534e)

- Once you click on "Create Pipeline," it will start running automatically. However, there's one setting we need to change to make sure it runs smoothly. Since we're not building any binaries or Docker images, we won't be using the "Build Artifacts" option. Because of this, we also need to update that setting in the Deploy stage.

![41](https://github.com/user-attachments/assets/fbb3d907-4329-4075-885d-2c9a1bc8e19b)
![42 5](https://github.com/user-attachments/assets/8ba82138-966e-4f45-b6a8-fc0e12f790a9)
![43 5](https://github.com/user-attachments/assets/5ada9626-99c2-4713-9744-220783a0f3f4)
![44 5](https://github.com/user-attachments/assets/ca1c9046-b025-4df8-a671-60d1d60ab61b)

- Change BuildArtifact to SourceArtifact and click on done.

![45 5](https://github.com/user-attachments/assets/f6ebe9e5-30ea-42af-99b5-c820242f1453)
![46 5](https://github.com/user-attachments/assets/a3a4710a-3546-4836-9e7e-10724a778b36)

- If You do not change the BuildArtifact to SourceArtifact, you'll get the below Error.

![43](https://github.com/user-attachments/assets/653a0c7d-a3ff-487b-a7c5-712e3f24d1bf)

- Make sure to update the SourceArtifact option. Sometimes, the pipeline might not run successfully on the first try because it automatically triggers as soon as you click "Create Pipeline." Unfortunately, you can't edit the SourceArtifact option during the pipeline setup. You'll need to manually adjust it after the pipeline is created.

- Once you've done that, you can trigger the pipeline by making changes in the repository.
  
![44](https://github.com/user-attachments/assets/dce93f2e-4ae0-446a-8734-ce47911047ae)

- After changes in the repo, the pipeline will be triggered again.
  
![46](https://github.com/user-attachments/assets/63524553-8e60-4690-b33a-624a22e3999c)
![47](https://github.com/user-attachments/assets/30007500-c597-456b-8295-ab02e9049ff6)

- The deployment went smoothly this time, with no errors. Here's the link to the project that's now up and running.
  
![output](https://github.com/user-attachments/assets/95e380c6-cc91-4fa6-8bdb-f03282638092)
