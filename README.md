# R training
https://departmentfortransport.github.io/R-cookbook/

## To contribute

1. Clone the repository
2. Make a new branch for your chapter or changes `git checkout -b name_of_branch`
3. Add/edit content in the `.Rmd` files. 
4. Create a pull request, get someone to review the content, and merge into master (merging into master will trigger the book website to be updated automatically).  Please do not include built files in your pull request.

## Using additional packages

If you wish to use a package not already loaded within the book then please add it to the imports section of the `DESCRIPTION` file.

### **lintR**

Please make sure that code sections pass [lintR](https://github.com/jimhester/lintr) checks.  Whilst currently linting errors won't stop the book from building we may in future change this and then any linting errors would cause the build to fail. This would be intentional to ensure the book does not contain any bad practices.

```R
lintr::lint('file.Rmd')
```

