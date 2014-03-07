# Text Errata

A List of errors and typos in the book
[Statistics, Data Mining, and Machine Learning in Astronomy](http://press.princeton.edu/titles/10159.html)

There are a couple ways to submit a new error report

- If you are a GitHub user, you can open a [Pull Request](https://help.github.com/articles/using-pull-requests) which edits this document.
- If you are not a GitHub user, please email the authors directly with your reported error, and we will add it to the list.


# Errata

Errors are listed by chapter, followed by page number.

## Chapter 1

Page 19 (also, Figure 1.2 on Page 21): The function `fetch_sdss_spectrum()`
does not, in fact, query any database in real time.  It simply retrieves a
specific file from the SDSS-I/II Data Archive Server (DAS) via http.

Page 35: Figure 1.13 is incorrectly labeled a Mercator projection.  It's actually an Equirectangular projection (also known in WCS as a "Cartesian projection")

## Chapter 2

Page 47/50: there are eight entries despite the title "Seven Strategies..."

Page 60: Eq. (2.7), "less than" sign should be "greater than"

## Chapter 3

Page 76: in Figure 3.3, the (1,1) and (2,2) cells are erroneously switched.

Page 99: The line below eq. (3.60) should say "Note that for k = 1 this distribution is a Cauchy distribution", not "k = 2"

Page 109: The first sentence in the paragraph preceeding eq. 3.78 should read
"If sigma_xy=0, then x and y are uncorrelated, and if also independent, we can
treat them separately as two one-dimensional distributions." (that is, vanishing 
correlation does not necessarily imply independence)


## Chapter 4

Page 126: The denominator of the argument of the exponential of Eq. (4.2) should be sigma squared, not sigma, to better match Eq. (3.43) and lead to Eq. (4.4).

Page 130: The denominator of the argument of the exponential of Eq. (4.11) should be sigma squared, not sigma, to better match Eq. (3.43) and lead to Eq. (4.13).


## Chapter 5

Page 221: In the sentence immediately preceding Eq. (5.100) the words
'and \mu' should be deleted.

## Chapter 6



## Chapter 7



## Chapter 8



## Chapter 9



## Chapter 10

Page 427: in the first paragraph of section 10.3.1, it should be
         omega = 2 pi f = 2 pi / P, and not (2 pi P) for the last part.

Page 437: figure 10.15: in the creation of this figure, the noise was not applied
to the data before computing the periodogram.  See a more detailed discussion along
with an updated figure on the
[astroML website](http://www.astroml.org/book_figures/chapter10/fig_LS_sg_comparison.html)



## Appendix

### Appendix A

### Appendix B

### Appendix C

Page 517:  The final paragraph of section C.3 should mention that SDSS does not
use Pogson magnitudes as defined in Equation C.2, but rather the asinh
magnitudes, see http://www.sdss3.org/dr10/algorithms/magnitudes.php#asinh.

Page 517: The SDSS magnitude system deviates from a perfect AB system by 0.01-0.02 mags. 
See http://www.sdss3.org/dr10/algorithms/fluxcal.php#SDSStoAB.

### Appendix D

Page 519: This query has to be submitted within a particular context within CasJobs, 
specifically DR8 or higher (DR7 does not have the value-added spectral information).

Page 519: The astrometric corrections of DR9 have not been applied to this query.
This affects the columns `G.ra` and `G.dec`. An additional join on the
`AstromDR9` table is necessary to get the correct astrometry (errors are <0.5 arcsec). 
See also http://www.sdss3.org/dr10/imaging/caveats.php#astrometry.

Page 519: The URL in the footnote is incorrect and it should be
http://skyserver.sdss3.org/casjobs/ (only the SDSS-III CasJobs site contains DR8 and higher
data).


### Appendix E
