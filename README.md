# Installing the app using a Scratch Org

1. Set up your environment. Follow the steps in the [Quick Start: Lightning Web Components](https://trailhead.salesforce.com/content/learn/projects/quick-start-lightning-web-components/).  The steps include:

    - Enable Dev Hub
    - Install Salesforce CLI
    - Install Visual Studio Code
    - Install the Visual Studio Code Salesforce extensions

1. If you haven't already done so, authorize with your hub org and provide it with an alias (myhuborg in the command below):
   
    ```
    sfdx auth:web:login -d -a myhuborg
    ```

1. Clone the sfdx-helloworld repository:
  
    ```
    git clone https://github.com/clintonharwood/sfdx-helloworld
    cd sfdx-helloworld
    ```

1. Create a scratch org and provide it with an alias (apex-recipes in the command below):
   
    ```
    sfdx force:org:create -s -f config/project-scratch-def.json -a sfdx-helloworld
    ```

1. Push the app to your scratch org
    
    ```
    sfdx force:source:push
    ```

1. Open the scratch org

    ```
    sfdx force:org:open
    ```
