# GitHub Page

## Modifying contents
- As of now, the site will only show Bio/contact
- Other sections, e.g. blogs, publications, are to be readded
- The md files in `content/home` can be turned on/off using
```
-active: true
```
- the header of the page can be added/remove in `config/_default/menus.yaml`
- the profile details is at `content/authors/admin/_index.md`
- general congif file at `config.yaml`
- Important: baseurl and publishdir must be changed to correspond to the site

## Publishing the site

```{r}
# to update the changes and publish the content
blogdown::build_site()

# to test the site locally
blogdown::serve_site()

# to stop the server
blogdown::stop_server()
```
- The updated content will be saved at `public/` (if the parameter `publishdir` was not set)
- In my case, the `publishdir` was set to `../{site}.github.io` and it has a separate git repo, which is pushed to https://github.com/izepb/izepb.github.io

## Useful guidelines
- https://evamaerey.github.io/what_how_guides/academic_website_w_blogdown
- https://bookdown.org/yihui/blogdown/github-pages.html 