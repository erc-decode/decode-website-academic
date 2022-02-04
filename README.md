# Customizations




## Job pages


### locations

* $ROOT/layouts/partials/
* $ROOT/layouts/partials/job/


### page_header.html

* Replaced the statements '{{ partial "page_metadata" (...) }}' in lines 68 and 95 by appropriate if...else constructs to distinguish job and other pages.


### job/page_metadata.html

We customize this file to display non-standard page metadata for job offers.

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




## Contact page


### contact.html

* Location: $ROOT/layouts/partials/widgets/
* This replaces the theme's standard contact widget by a very simple custom one that is a slight extension of the blank widget and is inspired by parts of the original contact widget.
* Note that we cannot give it a different name (like contact-lite.html), since then the two-column mode is not available (cf. line 120 in the original widget_page.html partial).


### get_address.html

* Location: $ROOT/layouts/partials/functions/
* With respect to the original file, we add two lines after line 20 in order to also deal with the custom address fields 'name' and 'institute'.


### address_formats.toml

* Location: $ROOT/data/
* We add one line in the beginning of the original file, which defines our custom address format called 'de-custom'.
* We tell the website to use this custom format by specifying it in $ROOT/config/_default/params.yaml.
