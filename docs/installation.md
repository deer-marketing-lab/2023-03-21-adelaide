# Software Installation

You will need to install the necessary software on to your laptop or personal computer to bring to work through the coding portions of this class.

!!! tip "Thanks Tilburg Science Hub!"
    These installation instructions have been made simpler by borrowing from [Tilburg Science Hub](https://tilburgsciencehub.com/).
    Check out their website for a tonne of cool stuff!

## R and R Studio

Throughout the course, we'll use R - a comprehensive toolbox to handle and analyze large data sets. 
The best thing about R is that it’s open source. 
It's freely usable by anyone. 
Plus there's a vibrant community that keeps on developing R. 

* Please install R and RStudio, by following these [setup instructions](http://tilburgsciencehub.com/get/r/).
  * Ignore any instructions about Path settings on Windows and Mac

<!-- Some OS specific extras: -->

<!---
* **Mac Users** 
    * Non M1 (older): Install the [Rtoolchain](https://github.com/rmacoslib/r-macos-rtools#installer-package-for-macos-r-toolchain-). This will automatically take care of several steps like installing Xcode, etc.  
    * M1 (newer): While the new M1 chips offer incredible performance, unfortunately they require several finicky steps to play nicely with
		some of the other tools that we might adopt. Please install Xcode by opening your Terminal and running `xcode-select --install`.
* **Windows Users**
    * Also install [Rtools](https://cran.r-project.org/bin/windows/Rtools/).

---> 

## R packages 

Throughout the course we'll need to install R packages to get some extra functionality.
Open RStudio and copy and paste this code chunk into the console:

```{r}

to_install <-
    c('tidyverse', 
        'tidytext',  
        'tokenizers', 
        'reshape2', 
        'wordcloud', 
        'vader',
        'stm',
        'yardtick',
        'textstem',
        'textdata',
        'stringr'
    )

install.packages(to_install)
```

This might take a while, so **please do this before coming to the workshop**.