## Purpose

This is a repository to host the source files for [my blog](https://jvadams.rbind.io/) powered by [Hugo](https://gohugo.io/) and [blogdown](https://bookdown.org/yihui/blogdown/).

## Adding posts

In December 2019, I ran into a snag using the [RStudio](https://rstudio.com/) Addin, Serve Site, aka `blogdown::serve_site()`.  I've not yet found a fix for the error,

    Error in shell(cmd, mustWork = TRUE, intern = intern) : 
      '"C:\Users\myname\AppData\Roaming\Hugo\hugo.exe" -b / -D -F -d "public" --themesDir themes -t hugo-lithium-theme' execution failed with error code 1

but I've got a workaround for adding new posts:  

- Start RStudio
- Addins, New Post
- Edit Rmd file
- knit
- Restart RStudio
- Addins, Serve Site
- GitHub Desktop, Commit to master, Push
