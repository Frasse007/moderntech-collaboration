**1. What triggers this workflow to run? (Look at the on: section)**  
A push or pull request to the "main" branch triggers the workflow to run.

**2. What are the four main steps this workflow performs? (List each step name)**  
It 1. Gets the code from the repository, 2. Validates the HTML files, 3. Checks for any broken links in the files, 4. Uploads the built site for deployment.

**3. What does the "Checkout code" step do and why is it necessary?**  
Gets the current version of code in the repository on the "main" branch in order to test it and then build with it.

**4. What is the purpose of the environment configuration?**  
It defines target environment metadata and sets the deployment URL. This allows GitHub to track deployment history and link the live site directly in the repository's main view

**5. How does this automated deployment improve reliability compared to manual deployment?**  
It eliminates human error by running consistent, standardized checks (HTML validation and link checking) on every single update before deploying. It prevents broken code or dead links from reaching production automatically.

**6. What would happen if you pushed code to a different branch (not main)?**  
The workflow would not run so nothing being outlined in it would be done. It would just be like pushing code to any repository without a workflow present.