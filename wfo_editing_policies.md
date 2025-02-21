# Tips and policies for working on Salicaceae nomenclature and taxonomy in Rhakhis

_Campbell O. Webb and Quentin Cronk_

(_Salix_ will be used as the exemplar genus in what follows)

See also the main Rhakhis [handbook][3].  Feel free to use the
[sandbox][4] (Staging Server) to fully explore the system, including
creating dummy names. All changes in the sandbox are overwritten
daily.

Nomenclatural elements of the data are in gray borders, while
taxonomic elements are in orange borders.  The following notes cover
the former first.

## Author String

Abbreviations should use Brummitt & Powell, Authors of Plant Names
(1992). IPNI can be used to search for the correct abbreviation. See
the [IPNI FAQs][1] for more information.

## Publication

Imported from IPNI and should be correct. Optimal form: `{Abbreviated
journal or book name}` `SPACE` `{(optional) {Volume} COLON SPACE}`
`{Page}` `PERIOD SPACE OPEN-PARENTHESIS` `{Year of publication}`
`CLOSE-PARENTHESIS`. See ‘IPNI Notifier’ below. See the [IPNI FAQs][2]
for more information.

## Nomenclatural References

Most of these should already be populated with literature and people.
At a minimum there should be a link to the protologue.  If one has the
details of the protologue, but cannot find a URL for an online
document, create a Wikidata entry. If one has a PDF of the protologue,
upload the PDF to Zenodo and use that DOI as the link.

### Type specimens

It is desirable that a link to an online representation of a type
specimen is provided for all accepted names, and for all basionyms.
The kind of type should be specified in the comments field of the
link.

## Nomenclatural Status

In order to switch the nomenclatural status of a name from ‘unknown’
to ‘valid’ or another option one **must** actively research the
name. However, considering the time required to perform this research
for the many names that need to be reviewed, it is only required to
check the status for names that are _accepted_ and that are currently
in an ‘unknown’ state.

Note that before adding a synonym to an accepted taxon, the status of
the accepted name must be ‘valid’ (or possibly ‘conserved’).

## Homotypic names

This box is computed by Rhakhis. The only option is to add or remove a
basionym. If a basionym is specified, all other names that share that
basionym are also listed.

## Placement

This is the main tool for assigning a taxonomic status. New names, and
many existing _Salix_ names, are unplaced (anywhere in the WFO
taxonomy), denoted by the gray bar above the name.

To accept a name, first the nomenclatural status must be either
‘valid’ or ‘conserved’. The option will appear in the placement
dropdown to ‘Raise to accepted taxon within...’, and _Salix_ (or a
_Salix_ species) can then be chosen.  The bar above the name will
change to orange (i.e., now a taxonomic entity, not just a
nomenclatural entity).
   
To make a name into a synonym of an accepted name, use the ‘Sink into
synonymy with...’ option. This is allowed even if the name’s
nomenclatural status remains ‘unknown’ (see above).
   
To move the accepted taxon from one name to its current synonym, first
raise the synonym to an accepted taxon with _Salix_, then sink the
currently accepted name into synonymy.

Do not move an unplaced infraspecific name into synonymy with a
species based solely on sharing a specific epithet with that
species. Some taxonomic knowledge or research is needed.

## Taxonomic Sources

Should be interpreted as taxonomic placement “according to...”

Every accepted and synonymous _Salix_ name should have at least one
entry in this list, _unless_ the decision to place a name is a new one
in which case the Wikidata URL of the person(s) making this decision
should be used as the source ([Quentin][5], [Cam][6]).  It is unlikely
will be making many new decisions about accepted taxa, but we may need
to make new decisions about obscure, unplaced synonyms. A full
discussion of a new decision is required in the Comments section.
 
The accepted name should not have a source for each of its synonyms;
each of the synonyms should have its own “according to” source.

The earliest published statement by an author about the taxonomic
placement of a name should be used as the primary entry, with
subsequent (flora, etc.) statements added if time allows.

Where various authorities agree, several entries should made. Where
authorities disagree, the link to the disagreeing authority should be
in the Other Treatments field, not here.

If the decision to accept is the same as the protologue in
Nomenclatural Source, that entry should be added to the Taxonomic
Source as well.

Common (type = Literature) options will be:

 * **Flora of North America** Display text: “Argus, G.W., et
     al. 2010. Salicaceae. Flora of North America 7: 23-162.”  URL:
     link to the online flora page,
     e.g. <http://floranorthamerica.org/Salix_alaxensis>.
      
 * **Dorn 2010** Display text: “Dorn, R.D. 2010, The Genus Salix in
     North America North of Mexico” URL:
     <https://www.lulu.com/shop/robert-dorn/the-genus-salix-in-north-america-north-of-mexico/ebook/product-6517733.html>
   
 * **Robert Dorn (in litt.)** Display text: “Robert Dorn (in litt.)”
     URL: <https://www.wikidata.org/wiki/Q2894282> Comments: “Robert
     Dorn’s review of N. American Salix communicated to Quentin Cronk
     and Campbell Webb via email (2024)”

POWO treatments (many originating from Irina Belyaeva) are classed as
‘Database’ entries.

## Other treatments

Use this for any other mentions of this taxon, either taxonomic
treatments that disagree with the placement chosen by us, or floras
that use a name.

## Comments

The stand-alone Comments field should be used for clarifying
information about the history and taxonomic status of the record, as
in the nomenclatural section of a published treatment.  This
discussion may combine comments on:

 * The original use of the name and authors in the protologue (i.e.,
   Nomenclatural References),
   
 * The editors’ own choice to accept or reject a particular
   publication as the source of the taxonomic placement (Taxonomic
   Sources),
   
 * Disagreement among authors concerning the taxon’s placement
   (disagreeing publications should be in Other Treatments)

Publications should be cited using a ‘Smith (2001)’ format, and all
discussed publications must be listed somewhere on the page.

The mini-discussion should be signed by following it with
`[XX, 2025-02-20]` (where XX is the reviewer initials, e.g., ‘QC’ or
‘CW’).

_Do not_ use the Comments field in the ‘Add Reference’ popup for the
above discussion. That reference-specific comment should be used only
for some comment about the reference/publication/database itself
(e.g., its availability).

### Tracking our review status

Rather than maintaining a separate tracking document or database, we
can indicate the state of reviewing using one of two strings in the
Comments section: `[Review in progress, XX, 2025-01-30]` or
`[Review complete, XX, 2025-01-30]` where XX is the reviewer initials,
e.g., ‘QC’ or ‘CW’.  If a record is visited several times before being
‘done’ the date of the ‘Review in progress’ should be updated.

## IPNI Notifier

IPNI author strings and publication citation strings are imported
regularly and _overwrite_ the values in Rhakhis. If a change is made
to either the author string or citation string, it is vital to notify
IPNI to ask them to update their data.

Since changing IPNI records is laborious for us and them, minor
variants in the IPNI citation string should be tolerated. Examples
include the publication year not in parentheses, or an extra page
range added to the treatment page (e.g., ‘505 (-507)’).  True errors
should always be corrected.

Template for email to IPNI:

ipnifeedback@kew.org


    ID number of plant/Author/Publication number
    Literature links (from e.g. BHL, GALLICA or Bibliotheca Digital), or
    Link to desired change/evidence
    A PDF or an image of a protologue.


## How to handle conflicting authorities

As WFO editors we are attempting to find a community consensus on
accepted names, but without taking too long.  Some independent
judgment calls will be required, and as long as the reasons for
decisions are documented in the Taxonomic Sources field and the
Comments field, these decisions can be further discussed and edited.
However, where a major conflict exists for a widespread taxon, we
should take our time.  In the case of North American taxa, this is
most likely to occur when Robert Dorn and George Argus disagree, and
in the case of taxa that occur on other continents and go by different
names there (e.g., _Salix bebbiana_).  While we review the evidence, a
note should be added to the Comments section indicating the nature of
the conflict.

[1]: https://www.ipni.org/about#about-authors
[2]: https://www.ipni.org/about#about-the-publication-dataset
[3]: https://plant-list-docs.rbge.info/rhakhis/
[4]: https://rhakhis.rbge.info/rhakhis/ui/index.html
[5]: https://www.wikidata.org/wiki/Q16298580
[6]: https://www.wikidata.org/wiki/Q45342779
