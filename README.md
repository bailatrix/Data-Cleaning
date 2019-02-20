# Data-Cleaning
Based on specifications from: https://makingnoiseandhearingthings.com/2018/04/19/datasets-for-data-cleaning-practice/
List of datasets:

Hourly Weather Surface – Brazil (Southeast region)
PhyloTree Data
International Comprehensive Ocean-Atmosphere Data Set
CLEANEVAL: Development dataset
London Air
SO MUCH CANDY DATA, SERIOUSLY
Production and Perception of Linguistic Voice Quality
Australian Marriage Law Postal Survey, 2017
The Metropolitan Museum of Art Open Access
National Drug Code Directory
Flourish OA
WikiPlots
Register of UK Parliament Members’ Financial Interests
NYC Gifted & Talented Scores
Hourly Weather Surface – Brazil (Southeast region)
It’s covers hourly weather data from 122 weathers stations of southeast region (Brazil). The southeast include the states of Rio de Janeiro, São Paulo, Minas Gerais e Espirito Santo. Dataset Source: INMET (National Meteorological Institute – Brazil).

Issues: Can you predict the amount of rain? Temperature? NOTE: Not all weather stations started operating since 2000

PhyloTree Data
Updated comprehensive phylogenetic tree of global human mitochondrial DNA variation. Human mitochondrial DNA is widely used as tool in many fields including evolutionary anthropology and population history, medical genetics, genetic genealogy, and forensic science. Many applications require detailed knowledge about the phylogenetic relationship of mtDNA variants. Although the phylogenetic resolution of global human mtDNA diversity has greatly improved as a result of increasing sequencing efforts of complete mtDNA genomes, an updated overall mtDNA tree is currently not available. In order to facilitate a better use of known mtDNA variation, we have constructed an updated comprehensive phylogeny of global human mtDNA variation, based on both coding‐ and control region mutations. This complete mtDNA tree includes previously published as well as newly identified haplogroups.

Issues: This data would be more useful if it were in the Newick tree format and could be read in using the read.newick() function. Can you help get the data in this format?

International Comprehensive Ocean-Atmosphere Data Set
The International Comprehensive Ocean-Atmosphere Data Set (ICOADS) offers surface marine data spanning the past three centuries, and simple gridded monthly summary products for 2° latitude x 2° longitude boxes back to 1800 (and 1°x1° boxes since 1960)—these data and products are freely distributed worldwide. As it contains observations from many different observing systems encompassing the evolution of measurement technology over hundreds of years, ICOADS is probably the most complete and heterogeneous collection of surface marine data in existence.

Issues: The ICOADS contains O(500M) meteorological observations from ~1650 onwards. Issues include bad observation values, mis-positioned data, missing date/time information, supplemental data in a variety of formats, duplicates etc.

CLEANEVAL: Development dataset
CLEANEVAL is a shared task and competitive evaluation on the topic of cleaning arbitrary web pages, with the goal of preparing web data for use as a corpus, for linguistic and language technology research and development. There are three versions of each file: original, pre-processed, and manually cleaned. All files of each kind are gathered in a directory. The file number remains the same for the three versions of the same file.

Issues: Your task is to “clean up” a set of webpages so that their contents can be easily used for further linguistic processing and analysis. In short, this implies:

removing all HTML/Javascript code and “boilerplate” (headers, copyright notices, link lists, materials repeated across most pages of a site, etc.);
adding a basic encoding of the structure of the page using a minimal set of symbols to mark the beginning of headers, paragraphs and list elements.
London Air
The London Air Quality Network (LAQN) is run by the Environmental Research Group of King’s College London. LAQN stands for the London Air Quality Network which was formed in 1993 to coordinate and improve air pollution monitoring in London. The network collects air pollution data from London boroughs, with each one funding monitoring in its own area. Increasingly, this information is being supplemented with measurements from local authorities surrounding London in Essex, Kent and Surrey, thereby providing an overall perspective of air pollution in South East England, as well as a greater understanding of pollution in London itself.

Issues: Lots of gaps (null/zero handling), outliers, date handling, pivots and time aggregation needed first!

SO MUCH CANDY DATA, SERIOUSLY
Candy hierarchy data for 2017 Boing Boing Halloween candy hierarchy. This is survey data from this survey.

Issues: If you want to look for longitudinal effects, you also have access to previous datasets. Unfortunate quirks in the data include the fact that the 2014 data is not the raw set (can’t seem to find it), and in 2015, the candy preference was queried without the MEH option.

Production and Perception of Linguistic Voice Quality
Data from the “Production and Perception of Linguistic Voice Quality” project at UCLA. This project was funded by NSF grant BCS-0720304 to Prof. Pat Keating, with Prof. Abeer Alwan, Prof. Jody Kreiman of UCLA, and Prof. Christina Esposito of Macalester College, for 2007-2012.

The data includes spreadsheet files with measures gathered using Voicesauce (Shue, Keating, Vicenik & Yu 2011) for both acoustic measures and EGG measures. The accompanying readme file provides information on the various coding used in both spreadsheets.

Issues: The following issues are with the acoustics measures spreadsheet specifically.

xlsx format with meaningful color coding created by a VBA script (which is copy-pasted into the second sheet)
partially wide format instead of long/tidy, with a ton of columns split into different timepoints
line 6461 has another set of column headers rather than data for some of the columns starting with “shrF0_mean”. I think this was a copy-paste error. Hopefully it doesn’t mean that all of the data below that row is shifted down by 1!
Australian Marriage Law Postal Survey, 2017
Response: Should the law be changed to allow same-sex couples to marry?

Of the eligible Australians who expressed a view on this question, the majority indicated that the law should be changed to allow same-sex couples to marry, with 7,817,247 (61.6%) responding Yes and 4,873,987 (38.4%) responding No. Nearly 8 out of 10 eligible Australians (79.5%) expressed their view.

All states and territories recorded a majority Yes response. 133 of the 150 Federal Electoral Divisions recorded a majority Yes response, and 17 of the 150 Federal Electoral Divisions recorded a majority No response.

Issues: Miles McBain discusses his approach to cleaning this dataset in depth in this blog post.

The Metropolitan Museum of Art Open Access
The Metropolitan Museum of Art provides select datasets of information on more than 420,000 artworks in its Collection for unrestricted commercial and noncommercial use. To the extent possible under law, The Metropolitan Museum of Art has waived all copyright and related or neighboring rights to this dataset using Creative Commons Zero. This work is published from: The United States Of America. You can also find the text of the CC Zero deed in the file LICENSE in this repository. These select datasets are now available for use in any media without permission or fee; they also include identifying data for artworks under copyright. The datasets support the search, use, and interaction with the Museum’s collection.

Issues: Missing values, inconsistent information, missing documentation, possible duplication, mixed text and numeric data.

National Drug Code Directory
The Drug Listing Act of 1972 requires registered drug establishments to provide the Food and Drug Administration (FDA) with a current list of all drugs manufactured, prepared, propagated, compounded, or processed by it for commercial distribution. (See Section 510 of the Federal Food, Drug, and Cosmetic Act (Act) (21 U.S.C. § 360)). Drug products are identified and reported using a unique, three-segment number, called the National Drug Code (NDC), which serves as a universal product identifier for drugs. FDA publishes the listed NDC numbers and the information submitted as part of the listing information in the NDC Directory which is updated daily.

The information submitted as part of the listing process, the NDC number, and the NDC Directory are used in the implementation and enforcement of the Act.

Issue: Non-trivial duplication (which drugs are different names for the same things?).

Flourish OA
Our data comes from a variety of sources, including researchers, web scraping, and the publishers themselves. All data is cleaned and reviewed to ensure its validity and integrity. Our catalog expands regularly, as does the number of features our data contains. We strive to maintain the most complete and sophisticated store of Open Access data in the world, and it is this mission that drives our continued work and expansion.

A dataset on journal/publisher information that is a bit dirty and might make for great practice. It’s been a graduate student/community project: http://flourishoa.org/

Issues: Scraped data, has some missing fields, possible duplication and some encoding issues (possibly multiple character encodings).

WikiPlots
 

The WikiPlots corpus is a collection of 112,936 story plots extracted from English language Wikipedia. These stories are extracted from any English language article that contains a sub-header that contains the word “plot” (e.g., “Plot”, “Plot Summary”, etc.).

This repository contains code and instructions for how to recreate the WikiPlots corpus.

The dataset itself can be downloaded from here: plots.zip (updated: 09/26/2017). The zip file contains two files:

plots: a text file containing all story plots. Each story plot is given with one sentence per line. Each story is followed by on a line by itself.
titles: a text file containing a list of titles for each article in which a story plot was found and extracted.
Issues: Some lines may be cut off due to abbreviations. Some plots may be incomplete or contain surrounding irrelevant information.

Register of UK Parliament Members’ Financial Interests
The main purpose of the Register is to provide information about any financial interest which a Member has, or any benefit which he or she receives, which others might reasonably consider to influence his or her actions or words as a Member of Parliament.

Members must register any change to their registrable interests within 28 days. The rules are set out in detail in the Guide to the Rules relating to the Conduct of Members, as approved by the House on 17 March 2015. Interests which arose before 7 May 2015 are registered in accordance with earlier rules.

The Register is maintained by the Parliamentary for Commissioner for Standards. It is updated fortnightly online when the House is sitting, and less frequently at other times. Interests remain on the Register for twelve months after they have expired.


Issues: Each member’s transactions are on a separate webpage with a different text format, with contributions listed under different headings (not necessarily one per line) and in different formats. Will take quite a bit of careful preprocessing to get into CSV or JSON format.

NYC Gifted & Talented Scores
Couple of messy but easy data sets: NYC parents reporting their kids’ scores on the gifted and talented exam, as well as school priority ranking. Some enter the percentiles as point scores, some skip all together, no standard preference format, etc. Also birth quarter affects percentiles.

2017 – 2018 results
2018 – 2019 results
