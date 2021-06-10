# flipbook_hex
an animated flipbook of how to make a hex map with rstats

The flipbook contents are defined in `build_hex.Rmd` using `data/temperature_obs_conus.csv`. The gif output is created using a combination of `flipbookr` + `xaringan` + `pagedown` + `magick`. Essentially, `xaringan` slides are made with an `.Rmd` using operations from `flipbookr` to define how the code is re-built, including paired code and graphics, highlighting, and sequencing.

To run locally use moon reader, may take ~10 min to knit. 
**Not yet working:** To produce a gif, can use `pagedown` to create frames from slides and animate with `magick`. To create the gif output, run the `flipbook_to_gif` function in `build_gif.R`. This process is based off of this github repo by [brshallo](https://github.com/brshallo/flipbookr-gifs-examples).

Because of the way the code build is written, it is easiest to troubleshoot the flipbook in pieces rather than re-knitting the `.Rmd`. This is partially due to the way the code progression is written. Still learning the ways! 

This flipbook is inspired by a [blog post by Shannon Pileggi for RLadies](https://www.pipinghotdata.com/posts/2021-03-08-r-ladies-styled-code-gifs-with-xaringan-and-flipbookr/) and the workflow is heavily based on examples in the [flipbookr documentation](https://github.com/EvaMaeRey/flipbookr#template) and [this blog post by Evangeline Reynolds](https://evamaerey.github.io/little_flipbooks_library/about/what_the_flipbook).
