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
