# 📚 Devops for Developers Notes - Java Techie #

## Index:
1. [Basic Introduction and Getting Started with Jenkins - ___18 Feb 2024___](#heading-1 "Basic Introduction and Getting Started with Jenkins - ___18 Feb 2024___")
2. [Jenkins Installation Guide for Windows and Mac - ___24 Feb 2024___](#heading-1 "Jenkins Installation Guide for Windows and Mac - ___24 Feb 2024___")



## Basic Introduction and Getting Started with Jenkins - ___18 Feb 2024___

### Simple flow (Manual approach) ###

- we write code -> store it in version control (GitHub) -> host in any cloud infrastructure- deploy the artifact (AWS, Azure, GCP)

- Before merging to GitHub, there should be pre-validation steps:
    - no compilation error
    - no build failure
    - no test failure
    - no major vulnerability

- We need to write script file and then deploy to cloud manually :(

- What if someone does the pre-validation task and deploy to cloud? Here comes Jenkins (We just need to instruct to Jenkins)

- Jenkins is an open-source automation server that facilitates the continuous integration and continuous delivery(CI/CD) of software. (automates ompilation, testing and deployment)

### Why Jenkins? (Problems before Jenkins) ###

- Manual Build and Deployment Processes
- Lack of Automated Testing (Unit tests, Integration tests)
- Inconsistency Across Environments(eg: version incompatibility in env)
- Deployment Challenges (deployment failure due to configuration mismatch)
- Poor Visibility and Monitoring (No tracking, no startup logs)

### What is CI/CD? ###

- Being a developer you only focus on development. Rest integration and deployment is taken care by Jenins

- Code -> GitHub -> (Compile->Build->Test->Code Scan)* -> Release(V1) -> Deploy

  *Will be taken care by Jenkins

> **Continuous Integration:** Code -> GitHub -> (Compile->Build->Test->Code Scan)</br> 
  **Continuous Delivery Deployment:** Release(V1) -> Deploy

<img src="assets/CI-CD.PNG" alt="ci cd" style="width: 60%;">

## Jenkins Installation Guide for Windows and Mac - ___24 Feb 2024___

### Installation Guide: ###
https://medium.com/@javatechie/jenkins-installation-steps-in-windows-mac-os-fcdc34b930c3

### CI/CD: ###
```
	                    Jenkins pipeline
  	            ------------------------------------
 CODE -> GITHUB -> [CLEAN, BUILD, TEST, SCAN] -> DEPLOY
                    ------------------------     ------
                              CI                   CD
                    ------------------------------------
```

- We need to create a pipeline to perform the whole CI/CD we call it Jenkins pipeline

- Pipeline: To execute sequence of action (both CI and CD)