# Tealium Cookie Match template for Google Tag Manager

## Overview

This is the Google Tag Manager template for the Tealium Cookie Match tag.

The Tealium Cookie Match tag template allows you to enable and configure vendor-specific cookie-match features for a number of vendors.  The following vendors are supported:
 - Centro
 - Criteo
 - DataXu
 - [Google Ad Manager (DoubleClick)](https://developers.google.com/authorized-buyers/rtb/cookie-guide)
 - MediaMath
 - [Salesforce Audience Studio (Krux)](https://konsole.zendesk.com/hc/en-us/articles/360000754674)
 - The Trade Desk
 - [Xandr (AppNexus)](https://wiki.xandr.com/display/supply/User+ID+Mapping)


The cookie match services will send the client-side visitor identifiers into Tealium for use with server-side Connectors in Tealium's Customer Data Hub (CDH).

For more information on Tealium's CDH, please visit [Tealium's Learning Community](https://community.tealiumiq.com/t5/Customer-Data-Hub/Introduction-to-Customer-Data-Hub/ta-p/17571)

## Quickstart Configuration

1. After adding the Tealium Collect Tag, search the Google Tag Manager Community Template Gallery for "Tealium Cookie Match"
2. Add this template
3. Create a new tag from this template
4. Enter the Tealium Account, Profile obtained from Tealium's CDH
5. Check the box for each vendor you wish to enable
6. Configure your Tealium Collect tag to run the Tealium Cookie Match tag *after* it fires [(as a "cleanup tag")](https://support.google.com/tagmanager/answer/6238868?hl=en)


## Additional Information

- The end user must have a browser that has enabled third-party cookies in order for these services to work.
- The Tealium Cookie Match tag will try again after 3 days to obtain the latest identifier (manually edit the template to adjust this threshold)
- The Tealium Cookie Match tag should run after the Tealium Collect tag in order to use the tealium_visitor_id value set from Tealium Collect

## Additional Resources

**[Documentation](https://community.tealiumiq.com/)**

## Copyright and license

Copyright 2020 Tealium Inc. All rights reserved.

Licensed under the **[Apache License, Version 2.0][license]** (the "License");
you may not use this software except in compliance with the License.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

