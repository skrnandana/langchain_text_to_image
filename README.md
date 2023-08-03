### Intern Name : Kavya Rama Nandana Sidda
### Alias : kavyarns
### Project Name : Text to Image Using Automatic Prompt Generator
### Project URL : https://github.com/skrnandana/langchain_text_to_image



### Project Description : The objective of this project is to deliver a Generative AI solution that enables advertisers to input text and receive a summary of the advertisement, caption for the advertisement and set of generated images to choose from. The solution meets the following business requirements:
+ Low to no human intervention
+ Scalable and cost effective
+ Receive appropriate content

Project is developed using AWS Serverless Application Model (AWS SAM). SAM is an open-source framework that developers use to build production-grade serverless applications on AWS.

### Prerequisites

+ [An AWS account] (https://aws.amazon.com/)
+ [AWS CLI installed and configured](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html#getting-started-install-instructions)
+ [Install SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html)
+ [Docker (For local testing)](https://www.docker.com/products/docker-desktop/)
+ Python 3.9
+ Any Integrated development environment (IDE).

### Installation
Steps to set up the project :

1. Clone the Repository
```
   git clone --recurse-submodules https://github.com/skrnandana/langchain_text_to_image.git

```

2. Configure aws credentials:
```
   aws configure

```

### Project Directory

langchain_text_to_image/
  |-- backend
    |-- octank-app
      |-- sam-template.yaml        
        |-- src/
          |-- app.py 
  |-- octankfrontend
    |-- amplify.yml                    


### Test and Deploy the project
1. Local Testing
  ```
  sam build
  sam local invoke -e <LambdaFunctionName> events/event.json

```

2. Deploy the SAM App
  ```
  sam build
  sam deploy --guided
