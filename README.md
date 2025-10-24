# ⚙️ AWS CI/CD Project

## 📘 Overview
This project demonstrates a **Continuous Integration and Continuous Deployment (CI/CD)** pipeline using **AWS** services — including **CodePipeline**, **CodeBuild**, **Elastic Beanstalk**, and **RDS** — with the source code hosted in **Bitbucket**.  

The primary goal of this project is to automate the build, test, and deployment process of a web application, ensuring faster, reliable, and consistent delivery of software updates.

---

## ❗ Problem Statement
Traditional software delivery methods rely heavily on manual deployment processes that are error-prone, time-consuming, and inconsistent across environments.  
As teams grow and application complexity increases, the lack of automation in build and deployment leads to:
- Deployment delays  
- Configuration drift between environments  
- Increased chances of human errors  
- Limited scalability and visibility in release cycles  

---

## 💡 Solution
To address these challenges, a **fully automated CI/CD pipeline** was implemented using **AWS Developer Tools** and **Bitbucket** as the source control system.  

This solution provides:
- **Continuous Integration** using **AWS CodeBuild**  
- **Continuous Deployment** via **AWS CodePipeline**  
- **Automated Environment Management** using **AWS Elastic Beanstalk**  
- **Managed Database Services** using **AWS RDS**  
- **Source Control Integration** through **Bitbucket** (migrated from GitHub)

The result is a **scalable, reliable, and automated CI/CD pipeline** that streamlines development workflows.

---

## 🎯 Objective
Build and deploy a fully automated **CI/CD pipeline** on **AWS** that:
- Integrates with **Bitbucket** for version control  
- Builds and tests the application using **AWS CodeBuild**  
- Deploys the application automatically to **Elastic Beanstalk**  
- Uses **AWS RDS** for persistent storage  
- Ensures minimal manual intervention for end-to-end delivery  

---

## 🧩 AWS Services Used

| *Service* | *Purpose* |
|------------|------------|
| **Bitbucket** | Source control and repository management |
| **AWS CodePipeline** | Automates CI/CD workflow — from source to deployment |
| **AWS CodeBuild** | Builds, tests, and packages application artifacts |
| **AWS Elastic Beanstalk** | Deploys and manages web applications automatically |
| **AWS RDS** | Provides managed relational database services for backend storage |

---

## 🏗️ Architecture

The architecture integrates **Bitbucket**, **CodeBuild**, **CodePipeline**, and **Elastic Beanstalk** for automated deployments.  

### 🧱 Architecture Description
1. **Bitbucket Repository (Code Source):**  
   The source code is hosted in Bitbucket — a **Git-based version control solution for professional teams** that supports collaboration through pull requests, code reviews, and branch management.  
   *(In this project, the repository was migrated from GitHub to Bitbucket.)*

2. **AWS CodePipeline:**  
   Acts as the automation backbone of the CI/CD process. It monitors the Bitbucket repository for changes and orchestrates the build and deployment stages.

3. **AWS CodeBuild:**  
   Responsible for compiling the code, running tests, and producing deployable artifacts. It ensures that each new commit is built and validated before deployment.

4. **AWS Elastic Beanstalk:**  
   Deploys the application in a managed environment. Elastic Beanstalk automatically handles provisioning, load balancing, scaling, and monitoring.

5. **AWS RDS:**  
   Used as the backend database layer for persistent data storage, ensuring scalability and reliability.

---

## ⚙️ Architecture Diagram  

![CICDArchitecture](https://github.com/user-attachments/assets/39ff7ddd-9aef-49d0-9696-7c95675a5ebd)


---

## 🔄 Workflow
1. Developer commits changes to **Bitbucket**.  
2. **AWS CodePipeline** detects the commit and triggers the pipeline.  
3. **AWS CodeBuild** compiles, tests, and builds the code.  
4. If successful, **AWS Elastic Beanstalk** automatically deploys the updated application.  
5. The application connects to **AWS RDS** for database operations.  
6. CI/CD automation ensures continuous delivery for every code push.

---

## 🧭 Migration from GitHub to Bitbucket
The source repository was migrated from **GitHub** to **Bitbucket** for enhanced integration with team workflows and pipeline automation.

### Migration Steps:
- Export repository from GitHub.  
- Import the repository into Bitbucket.  
- Update **AWS CodePipeline** to use Bitbucket as the source.  
- Verify successful connection and trigger pipeline execution.

---

## 🧪 Testing the CI/CD Flow

To test the pipeline after setup, execute standard Git commands:

# Make changes to your code
git add .
git commit -m "Testing CI/CD flow"
git push origin main

Once the code is pushed:

- **AWS CodePipeline** automatically starts.
- **AWS CodeBuild** compiles and tests the new code.
- **AWS Elastic Beanstalk** updates the running application if the build is successful.
- You can monitor each stage in the **AWS CodePipeline Console**.
  
---

## 🚀 Key Learnings

- Practical implementation of **AWS CI/CD pipeline**
- Automated **build, test, and deploy** using AWS Developer Tools
- Integration between **Bitbucket** and **AWS CodePipeline**
- Hands-on experience with **Elastic Beanstalk deployment automation**
- Understanding of **end-to-end DevOps workflows** on AWS

---

## 🧾 Future Improvements

- Integrate **Amazon CloudWatch** for real-time monitoring and alerts  
- Add **CodeDeploy** for advanced deployment strategies (Blue/Green)  
- Implement **Infrastructure as Code (IaC)** using **CloudFormation** or **Terraform**  
- Expand testing with **AWS CodeGuru** for code quality insights  

---
## 💬 About the Project

This project showcases a **complete CI/CD pipeline** on AWS — starting from **source code in Bitbucket** to **automated deployment in Elastic Beanstalk**.  
It exemplifies how **automation improves delivery speed**, **reduces manual effort**, and **ensures reliable deployments at scale**.

---

## 👩‍💻 Author
*Sakshi Sharma*  
📫 [Connect on LinkedIn] : www.linkedin.com/in/sakshisharma48
