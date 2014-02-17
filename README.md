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
See also [this pull request](https://github.com/astroML/astroML/pull/29).  As
"a simple example of the way SQL queries can be used with the SDSS database"
(page 21), Section 1.5.5 would be more appropriate.

Page 35: Figure 1.13 is incorrectly labeled a Mercator projection.  It's actually an Equirectangular projection (also known in WCS as a "Cartesian projection")

## Chapter 2

Page 47/50: there are eight entries despite the title "Seven Strategies..."

Page 60: Eq. (2.7), "less than" sign should be "greater than"

## Chapter 3

Page 76: in Figure 3.3, the (1,1) and (2,2) cells are erroneously switched.

Page 99: The line below eq. (3.60) should say "Note that for k = 1 this distribution is a Cauchy distribution", not "k = 2"

## Chapter 4

Page 126: The denominator of the argument of the exponential of Eq. (4.2) should be sigma squared, not sigma, to better match Eq. (3.43) and lead to Eq. (4.4).

Page 130: The denominator of the argument of the exponential of Eq. (4.11) should be sigma squared, not sigma, to better match Eq. (3.43) and lead to Eq. (4.13).


## Chapter 5



## Chapter 6



## Chapter 7



## Chapter 8



## Chapter 9



## Chapter 10

Page 427: in the first paragraph of section 10.3.1, it should be
         omega = 2 pi f = 2 pi / P, and not (2 pi P) for the last part.

Page 437: figure 10.15: in the creation of this figure, the noise was not applied
to the data before computing the periodogram.  See a fuller discussion along
with an updated figure on the
[astroML website](http://www.astroml.org/book_figures/chapter10/fig_LS_sg_comparison.html)



## Appendix

### Appendix A

### Appendix B

### Appendix C

Page 517:  The final paragraph of section C.3 should mention that SDSS does not
use Pogson magnitudes as defined in Equation C.2, but rather the asinh
magnitudes defined by [Lupton, Gunn & Szalay (1999)](http://adsabs.harvard.edu/abs/1999AJ....118.1406L).
See also http://www.sdss3.org/dr10/algorithms/magnitudes.php#asinh.

Page 517: The SDSS magnitude system is *almost* but not *exactly* on the
AB system.  There are ~1% differences.  See http://www.sdss3.org/dr10/algorithms/fluxcal.php#SDSStoAB.

### Appendix D

Page 519: This query has to be submitted within a particular context within
CasJobs, specifically DR8.

Page 519: The astrometric corrections of DR9 have not been applied to this query.
This affects the columns `G.ra` and `G.dec`. An additional join on the
`AstromDR9` table is necessary to get the correct astrometry.
See also http://www.sdss3.org/dr10/imaging/caveats.php#astrometry .

Page 519: The URL in the footnoate is incorrect.  It should be
http://skyserver.sdss3.org/casjobs/ .  Only the SDSS-III CasJobs site contains
DR8 data.


### Appendix E
