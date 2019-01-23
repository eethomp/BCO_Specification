_This document is part of the [BioCompute Object specification](bco-specification.md)_

_Back to [BCO domains](bco-domains.md)_

### 2.3.3 Extension to External References: License for data and script
    
The external references **example** extension to additional license, provides a mechanism for adherence to licensing requirements associated with the source code, software, scripts and data. The licenses provide a binding guideline for the use and distribution of such resources and authorizes the end user by granting specific rights to use them without violating any copyrights laws and rules. 

Depending on the license, certain licenses allow end user to share, modify, copy and redistribute the data and scripts whereas some liceses completely restrict the end user from modifying, copying, sharing and re-distributing the scripts and data.  Some licenses allow to copy, share and modify datasets and scripts but require proper attribution in doing so. Thus, additional_license plays a vital role in dataset BCO creation     

The `additional_license` extension is defined as an array of licenses applied to the data and the script. 

`data_license` is a string containing the URL of the license applied to the data or datasets. 

`scripts_license` is a string containing the URL of the license applied to the scripts.

Licenses of [Creative Commons](https://creativecommons.org/) can be applied to the data and licenses of [GNU](https://www.gnu.org/licenses/licenses.html) can be applied to the scripts, software or source codes. Additional information about the license can be added to the usability domain. 

```json
    "extension_domain":{
        "additional_license":{
            "data_license": "https://creativecommons.org/licenses/by/4.0/",
            "scripts_license": "https://www.gnu.org/licenses/gpl-3.0.en.html"
            }
```
