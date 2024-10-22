Exercise 1: Github Pipeline

1. A developer creates a new GitHub repository, which contains an Rmarkdown file that has an R code chunk defining a function with a single argument `data`, that takes a dataset and performs some input transformation on it. This transformation can be as simple or complex as you like, but should work on at least one dataset (either a built-in R dataset, or one provided by you in the public repository). The function should return the transformed data.

2. The developer knits the Rmarkdown file, which generates an HTML file with the function inside a code chunk and the output of the function after running it on the dataset. The developer includes this knitted HTML file in the repository.

3. The developer wishes to a second function that does a different transformation, but also takes a single argument `data` (a dataset) and returns a transformed dataset. To preserve the integrity of the main branch, they add this functionality in a new branch called `dev`, which they do *not* immediately merge into main.

4. The developer then goes on holiday and gets an email from their supervisor asking them to rename the argument in the second function `data_new`. This seems like a very silly request, but the developer obliges. Since the developer does not have their computer handy, they make this small edit directly in the Rmarkdown file in GitHub. 

5. Once they are home, the developer knits the Rmarkdown file again, now containing the second function with the `data_new` argument, and including the updated knitted HTML file in the repo. The developer then merges the `dev` branch into `main` and deletes it.
