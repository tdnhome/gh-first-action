# gh-first-action



1. Log into https://github.com/

2. On the left panel, click on 'New' to create new repository
   2.1 Repository template: No template
   2.2 Repository name: any name
   2.3 Select Public (instead of Private)
   2.4 Check 'Add a README file' option
   2.5 Add .gitignore: None
   2.6 Choose a licence: None 

   Click 'Create' 
	
3. Click on Actions tab

   3.1 Simple workflow
   3.2 Configure
   3.3 Change the file first-action.yml (Note that it must be under /.gitgub/workflows)
   3.4 Clear the content of the file
   3.5 Add workflow below.  Note: pay attention on the line indents correctly.
   
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
