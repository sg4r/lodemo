# lodemo
Démo de l'utilisation de rblt 2.4.7

## réccuprer un dataspace d'exemple
```
git clone https://github.com/sg4r/lodemo.git
```
## depuis R studio
```
# definir le repartoire de travail dans le repo git
setwd("~/lodemo")

# install rblt dev version
install.packages("devtools")
devtools::install_github("sg4r/rblt")

# load rblt library
library("rblt")

# view 2 fichiers Cats
l=LoggerList$new()
l$add(LoggerCats$new("CC-07-47_14-02-2018_corr.h5"))
l$add(LoggerCats$new("CC-07-115_14-02-2019_corr.h5"))
lui=LoggerUI$new(l)
lui$gui()
```
