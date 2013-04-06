Report_eucalyptus_on_sierra
===========================

Prerequisite
------------
- phantomjs
- futuregrid/cloud-metrics

How to create report?
---------------------
``make report FROM_DATE=$your start date TO_DATE=$your end date``
example.
``make report FROM_DATE=2013-01-01 TO_DATE=2013-03-31``

open pdf file under _build/latex directory

How to modify pages?
--------------------

Edit sierra.rst file

It is restructuredText file to be generated in a html or pdf file using Python Sphinx

How to modify command?
----------------------

Edit data.txt or report_euca_sierra_201207to12.txt

The file has the list of commands to generate charts that included in the report.

Add Ons to be included
-----------------------

1) command to create a report by resource and period

report -resource sierra -service eucalyptus -from ??:??:?? -to ??:??:?? 

report -summary -resource sierra india -service eucalyptus openstack -from ??:??:?? -to ??:??:?? 
report -summary -resource sierra -service openstack -from ??:??:?? -to ??:??:?? 
report -summary -resource sierra -service eucalyptus -from ??:??:?? -to ??:??:?? 


possibly add format to the command 

-format pdf
-format sphinx
-format html       ?
