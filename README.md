![Familia Mongefranco Logo](https://avatars.githubusercontent.com/u/42566530?s=400&u=47b770f0042e87f559edaef88a68cae8529595d2&v=4 "mongefranco.com")

# Bluesky Feeds

## Description
Custom post feeds that can be used in the Bluesky micro-blogging platform. Fork this repo to start your own feeds, or simply open the published feed links to follow in the Bluesky app.


## Quick Start Guide
+ To add a feed to Bluesky, simply click on one of the feed links below and either pin it or subscribe to it.
+ To further customize a feed, or to build your own based on these custom feeds, open the apropriate JSON file and copy & paste into [Skyfeed.app](https://skyfeed.app).
  


## Available Feeds
### #umichresearch
<img src="images/umichresearch.png" alt="#umichresearch feed logo" title="#umichresearch feed" style="width: 120px;" width="120px" /><br />
Highlights from research, publications, discoveries and innovations at University of Michigan.
+ View this feed: https://bsky.app/profile/gabriel.mongefranco.com/feed/aaacxlaaujdck
+ View the code: [umichresearch.json](umichresearch.json)


## Documentation

### #umichresearch
1. Get all feeds (firehose) from the past 12 hours
2. Remove replies, leaving only posts and re-posts (to speed up filters that follow)
3. Filter using regular expressions (regex), searching the post text, images alt text, and links
4. + Match pattern "umich research", "umich center", etc.
     + Match the beginning of any word, or words starting with # or @
     + Then match umich, mich med, etc.
     + Then optionally match end of the word or apostrophe s ('s)
     + Then match health, center, institute, research, etc.
     + Then match optional endings in ing, ed, etc.
     + Then match the end of the word (word boundary)
   + OR match links to any sub-domains of umich.edu, umflint.edu or umdearborn.edu (the parent domains are excluded to avoid getting unrelated university announcements)
   + OR match links to specific domains that also contain research articles (e.g. michiganmedicine.org, myuofmhealth.org, depressioncenter.org)
5. Limit to 2000 results (since this could potentially return thousands of posts)
6. Add posts using any of the following tags: #umichresearch, #umich-research, #umichresearchers, #umich-researchers, #umichscience, #umdepressioncenter, #umichdepressioncenter, #umichmetric, #ummetricsymposium, #umichmetricsymposium, #metricsymposium, #umichisr, #d3center, #umichd3c, #umichpsc
7. Try to narrow posts by filtering using regular expressions for research-related keywords, or keywords that researchers are likely to use when referring to studies and research-related events
8. Then remove potentially offensive or off-topic (non-research) posts with an inverse regular expresison filter
9. Remove offensive, sexually charged, hate charged, misleading, or spam posts using the Bluesky Moderation Service
10. Remove duplicates
11. Finally, sort by creation date to display newest posts first

  

## Additional Resources
+ Bluesky micro-blogging platform: https://bsky.app
+ Skyfeed feed builder: https://skyfeed.app.
+ Bluesky API documentation: https://docs.bsky.app/



## About the Author
Gabriel Mongefranco is a Mobile Data Architect and Software Developer. Gabriel has over a decade of experience in API development, automation, backend development, data analytics, dashboard design, database design, middleware development and architecture, mobile data cleaning and analysis, and technical writing.



## Contact
To get in touch, please visit: https://gabriel.mongefranco.com.


## Credits
#### Contributors:
+ Gabriel Mongefranco [(@gabrielmongefranco)](https://github.com/gabrielmongefranco)



#### This work is based in part on the following projects, libraries and/or studies:
+ Skyfeed feed builder: https://skyfeed.app.


## License
### Copyright Notice
Copyright © 2024-2025 Gabriel Mongefranco


### Software and Library License
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/gpl-3.0-standalone.html>.


### Documentation License
Permission is granted to copy, distribute and/or modify this document 
under the terms of the GNU Free Documentation License, Version 1.3 
or any later version published by the Free Software Foundation; 
with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts. 
You should have received a copy of the license included in the section entitled "GNU 
Free Documentation License". If not, see <https://www.gnu.org/licenses/fdl-1.3-standalone.html>



## Citation
If you find this repository, code or paper useful for your research, please cite it.

----

Copyright © 2024-2025 Gabriel Mongefranco
