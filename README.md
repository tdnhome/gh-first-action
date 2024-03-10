# gh-first-action



1. Log into https://github.com/

2. On the left panel, click on 'New' to create new repository
   - Repository template: No template
   - Repository name: any name
   - Select Public (instead of Private)
   - Check 'Add a README file' option
   - Add .gitignore: None
   - Choose a licence: None 

   Click 'Create' 
	
3. Click on Actions tab
   - Simple workflow
   - Configure
   - Change the file first-action.yml (Note that it must be under /.gitgub/workflows)
   - Clear the content of the file
   
4. Code Add workflow below.  Note: pay attention on the line indents correctly.
```   
   name: First Workflow
   on: workflow_dispatch
   jobs:
     my-very-first-job: 
       runs-on: ubuntu-latest
       steps:
         - name: Print greeting
           run: echo "Hello World!"
         - name: Print goodbye
           run: echo "Done - Bye!"
```
Note on the "on: workflow_dispatch" text above.  It means there is no event that trigger this workflow and we will trigger the workflow execution manually.

5. Click on 'Start commit' to commit the first-action.yml file
   - Enter text for the commit's title
   - Enter text for the commit's description
   - Click on 'Commit new file'
  
6. Execute the 'first-action.yml' workflow
   - Click on Actions tab
   - Click on the 'First Workflow' on the left panel
   - Click on the 'Run workflow' button, select the branch and click on the 'Run workflow' to run the workflow
  
7. View workflow log
   - The workflow main panel contains the list of executed workflows
   - Click on the 'First Workflow' then click on the job on the workflow to see the job's log
      
