# spsDS

systemPipeShiny Data Science(spsDS) is a [systemPipeShiny](https://github.com/systemPipeR/systemPipeShiny) 
plugin that contains a variety of plot tabs(different interactive [Shiny](https://shiny.rstudio.com/) plots). 

An online demo of this plugin is provided here:

## Installation

```r
# stable version(haven't been pushed to CRAN yet)
# install.packages("spsDS")
# develop version 
remotes::install_github("lz100/spsDS")
```

## Quick start

To use this plugin, first create a SPS project:

```r
# replace "YOUR_PROJECT_NAME" to a meaningful name
library(systemPipeShiny)
spsInit(project_name = "YOUR_PROJECT_NAME")
```
Now test if the app can be run by typing shiny::runApp() in console or click 
on the green `> Run App` button on top right corner if you open the *global.R*.

If the app runs, stop the app and load the plugin:

```r
spsAddPlugin("spsDS")
```

In the *global.R* file under the project root add `plugins = c("spsDS")` and you 
can run the app. 

```r
sps_app <- sps(
    vstabs = "",
    plugins = c("spsDS"),
    server_expr = {
        msg("Custom expression runs -- Hello World", "GREETING", "green")
    }
)
```
## Plot options
This is a gallery of screenshots of what plots this plugin can make. 

Update later...

## Contribution

Submit a pull request to contribute with more plot options(tabs).

## License 

[MIT](https://github.com/lz100/spsDS/blob/master/LICENSE.md)
