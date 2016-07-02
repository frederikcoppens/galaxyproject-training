# Best Practice Sharing Galaxy Workflows

## Make the workflow

* Make your workflow using e.g. the workflow editor or based on a history (link to info on making workflow?)
* Use tools that are available in a toolshed, preferable the main [ToolShed](https://toolshed.g2.bx.psu.edu), to ensure this make the workflow on usegalaxy.org
* Test your workflow with a sample dataset, preferably small enough to finish the whole procedure within minutes

## Export the workflow

* Go to the tab Workflow and click right on the workflow you want to export
* Select ‘Share or Download’
* In the section ‘Export’ click Download. This will download a Galaxy-workflow-name-of-your-workflow.ga file to your computer 
* You can also download an image as SVG, this will open a new tab (depending on the settings of your browser). Click right on the figure and save it as Galaxy-workflow-name-of-your-workflow.svg

## Make all files available

* Make a (folder in a) GitHub repository to contain all files relevant for this workflow (link how to make GitHub account ? )
* Add the Galaxy-workflow-name-of-your-workflow.ga file
* Create a readme.rst file ([example](https://github.com/galaxy-scientists/galaxyproject-training/blob/master/GCC2016_workflow/readme.rst))
* Create a file ‘repository_dependencies.xml’ containing the dependencies ([example](https://github.com/galaxy-scientists/galaxyproject-training/blob/master/GCC2016_workflow/repository_dependencies.xml)). Currently this needs to be done manually. Name and Owner can be found in the [ToolShed](https://toolshed.g2.bx.psu.edu) for all tools used in the workflow
* Create a folder ‘test-data’ and add all input files needed for a test run
* Create a folder ‘output-data’ and add output files for validation

## Publish workflow

* Create an account on the [ToolShed](https://toolshed.g2.bx.psu.edu) or [TestToolShed](https://testtoolshed.g2.bx.psu.edu)
* ‘Create new repository’ under ‘Available actions’ on the left
* Give it an appropriate name (only letters, numbers and underscores)
* Select ‘unrestricted’ type
* Fill in the link to the repository, synopsis, description
* Select an appropriate category
* Save

* Upload files (button right top)
	* Galaxy-workflow-name-of-your-workflow.ga
	* Readme.rst
	* Repository_dependencies.xml

## Provide the example dataset on usegalaxy.org

* Load the example data in a history on usegalaxy.org
	* Share this history, this is the starting point
* Make a copy of the history to a new one and run the workflow
	* Share also this history, this is the “answer” or final point
	
## Make an interactive tour

* Examples can be found [here](https://github.com/galaxyproject/galaxy-tours/)
* Add it to your github repo
* Getting it into usegalaxy.org requires a pull request… How to address this?

