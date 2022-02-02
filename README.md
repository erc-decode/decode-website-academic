# Customizations


## Job pages

### locations

* $ROOT/layouts/job/
* $ROOT/layouts/partials/job/


### single.html (compared to _default/single.html)

* Changed '{{ partial "page_header" . }}' to '{{ partial "job/page_header" . }}' in line 5.


### page_header.html

* Changed '{{ partial "page_metadata" (...) }}' to '{{ partial "job/page_metadata" (...) }}' in lines 68 and 95, thus pointing to the custom partial instead of the default one supplied by the Academic theme


### page_metadata.html

* Remove first block associated with author.
* Add "Closing date:" in front of the date to be displayed (second block).
* Remove third block associated with publication.
* Modified fourth block so that it is about "contract duration" instead of reading time.
* Remove fifth block associated with Disqus.
* Changed taxonomy from *categories* to *tags* in the sixth block
* Added an additional block associated with the link to the original job ad.

