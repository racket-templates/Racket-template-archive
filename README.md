# Racket templates
The Racket-templates archive for finding, uploading, and cloning templates.

## Using templates 
Using existing templates is easy. The first thing you have to do is install the templating tool: 
```
raco pkg install new
```
will install the templating tool for you. Then you can download any template you want by running 
```
raco new <template-name> <optional-folder-location>
```
You can view all available templates in this repository in the `templates` directory, or you can 
search them in your command line by doing 
```
raco new --list
```
to see all available templates.

## Creating a template
To create a template, you can use the existing template to create a new one - run 
```
raco new template <optional-folder-location>
```
and the command will create a new template for you based on the https://github.com/racket-templates/template template repository.


## Submitting a template

Once you've created your template, you can submit it here by creating a new 
pull request. Your pull request should contain a single file with the name of 
your template, with the following contents:
```scheme
(name <name of template>
 repo username/repo-name
 from [github|gitlab]
 desc "A short description of your template.")
```

A good example is [Rosette](https://github.com/racket-templates/rosette-template): 
```
(name rosette
 repo "racket-templates/rosette-template"
 from github
 desc "A #lang rosette template for program verification and synthesis.")
```

