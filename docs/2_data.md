---
title: "Data"
output: html_notebook
editor_options:
  chunk_output_type: inline
---

# Data



Data compiled and used in this project

## Data collection
We collect fecal samples of two primate and two bat species.

### Nyctalus noctula
Samples were collected by Lara Keicher, Dina Dechmann and colleagues during regular box monitoring at their field sites in Konstanz and Kreuzlingen.
Sample collection data was sent via email by Lara Keicher to Gisela on 30.4.2021 and is stored in `raw_data` as `Samples_Nycnoc_20210430.csv`.


```r
samplesNycnoc <- read.csv("vignettes/data/data_raw/Samples_Nycnoc_20210430.csv", header = TRUE, sep = ";", as.is = TRUE)

str(samplesNycnoc)
#> 'data.frame':	27 obs. of  52 variables:
#>  $ date                  : chr  "2021-04-22" "2021-04-22" "2021-04-22" "2021-04-22" ...
#>  $ season                : chr  "spring" "spring" "spring" "spring" ...
#>  $ location              : chr  "Kreuzlingen Seeburgpark" "Kreuzlingen Seeburgpark" "Kreuzlingen Seeburgpark" "Kreuzlingen Seeburgpark" ...
#>  $ roost                 : int  38 38 38 38 38 38 38 31 31 31 ...
#>  $ roost.type            : chr  "Wintertonne" "Wintertonne" "Wintertonne" "Wintertonne" ...
#>  $ box.exp               : logi  NA NA NA NA NA NA ...
#>  $ other.animals.in.roost: chr  "19+" "19+" "19+" "19+" ...
#>  $ time                  : chr  "day" "day" "day" "day" ...
#>  $ bat.id                : chr  NA NA NA "00079B133F" ...
#>  $ bag.nr                : chr  "A16" "K37" "A11" "K19" ...
#>  $ genus                 : chr  "Nyctalus" "Nyctalus" "Nyctalus" "Nyctalus" ...
#>  $ species               : chr  "noctula" "noctula" "noctula" "noctula" ...
#>  $ transmitter           : logi  NA NA NA NA NA NA ...
#>  $ tx.mass               : logi  NA NA NA NA NA NA ...
#>  $ tx.attachment         : logi  NA NA NA NA NA NA ...
#>  $ tx.time.on            : logi  NA NA NA NA NA NA ...
#>  $ recap                 : chr  "no" "no" "no" "no" ...
#>  $ mass.w.bag            : num  51 55 45 50 48 50 52 49 46 51 ...
#>  $ mass.of.bag           : num  24 25 20 24 23 25 24.5 26 20 24 ...
#>  $ mass.of.bat           : num  27 30 25 26 25 25 27.5 23 26 27 ...
#>  $ sex                   : chr  "f" "f" "f" "m" ...
#>  $ age                   : chr  "a" "a" "a" "a" ...
#>  $ FA.right              : num  54.3 NA NA NA 54.5 ...
#>  $ FA.left               : num  NA 54.7 53 55.4 NA ...
#>  $ repro.state           : chr  "nulli" "plac" "nulli" "scr" ...
#>  $ nipple                : chr  NA NA NA NA ...
#>  $ testes                : chr  NA NA NA "s" ...
#>  $ testes.size           : logi  NA NA NA NA NA NA ...
#>  $ bucchal.gland         : chr  NA NA NA NA ...
#>  $ streblids             : chr  "yes" "no" "no" "no" ...
#>  $ streblid.counts       : int  1 0 0 1 0 0 0 0 0 0 ...
#>  $ mites                 : chr  "yes" "yes" "no" "no" ...
#>  $ mite.counts           : int  3 2 0 0 0 0 0 0 0 1 ...
#>  $ other.parasites       : chr  "no" "no" "no" "no" ...
#>  $ parasites.coll.       : chr  "no" "no" "no" "no" ...
#>  $ wingpunch..Dna.MHC.   : chr  "no" "no" "yes" "yes" ...
#>  $ wingpunch.samples     : chr  "no" "no" "yes" "yes" ...
#>  $ isotopes              : chr  "no" "no" "no" "yes" ...
#>  $ fur.samples..isotopes.: chr  "no" "no" "no" "yes" ...
#>  $ feces                 : chr  "yes" "yes" "yes" "yes" ...
#>  $ foto                  : chr  "no" "no" "no" "no" ...
#>  $ blood.smear           : chr  "no" "no" "no" "no" ...
#>  $ blood.sample          : chr  "no" "no" "no" "no" ...
#>  $ vaginal.smear         : chr  "no" "no" "no" "no" ...
#>  $ teeth                 : int  0 1 1 0 0 0 1 1 1 0 ...
#>  $ Team                  : chr  "Lara, Dina, Edward, Jenna, Ellen" "Lara, Dina, Edward, Jenna, Ellen" "Lara, Dina, Edward, Jenna, Ellen" "Lara, Dina, Edward, Jenna, Ellen" ...
#>  $ comment               : chr  "wing tear" "" "" "" ...
#>  $ X                     : chr  "6 bats flew out" "6 bats flew out" "7 bats flew out" "7 bats flew out" ...
#>  $ X.1                   : logi  NA NA NA NA NA NA ...
#>  $ X.2                   : chr  "feces for Gisela" "feces for Gisela" "wingpunch and feces  for Gisela" "feces for Gisela" ...
#>  $ X.3                   : logi  NA NA NA NA NA NA ...
#>  $ X.4                   : logi  NA NA NA NA NA NA ...
```

:::beware
Need to check sample IDs and include in table!
:::


## Data processing


---
