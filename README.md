# NWB Metadata GUI

nwb-metadata-gui is a tool for generating a meta-data file that can be paired with an NWB conversion tool to
define meta-data you want to package inside the NWB file.

Often when converting data to NWB, the original data does not have meta-data that would be required
by NWB and/or DANDI, and often we want to add meta-data when sharing data publicly so that users
can understand the data better, to find it better, and to credit the original experimenters.
As a result, a large part of building conversion software to NWB is adding meta-data, particularly
when this data will be shared publicly. Some conversion tools are popping up where this meta-data is hard-coded
as text fields deep in the script. That solution works for one-off scripts.

This tool provides a structure for populating a json file with the meta-data that can go in an NWB file. It is 
meant to be paired with a conversion tool that can read this file and insert the meta-data in the appropriate places
while constructing an NWB file.
