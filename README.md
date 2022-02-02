# Customizations


## Job pages

### locations

* $ROOT/layouts/job/
* $ROOT/layouts/partials/
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


### page_metadata_authors.html

We customize this file to display the group name instead of the author's name whenever the author of a job offer is displayed (regardless of the chosen view).

* Introduce a new variable called $input_page_type in order to store the type of the underlying page to be linked to. We want to distinguish "job" pages from others.
* Introduce a new variable called $display_name, which is either set to the group name (for job pages) or to the author's name as before (otherwise).
* Note that in order to change the $display_name variable inside an if branch, we need to use the '=' instead of the ':=' assignment operator.

