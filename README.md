# Nice

Nice is a gradual webscraper, named nice because it tries to place nice with servers by not immediately downloading everything at once. Instead, it starts by downloading a skeleton of the page with a single level of recursion, and then prompts for further downloads as assets are needed. Thus, the end user only mirrors what they need and the bandwidth is not abused all at once.

## Method
For this to work, the static content of the page has to interact with a program on the system to request further downloads and modify HTML files as necessary. Therefore, it has to be a static webserver. When launching the site, three options can be provided:

- Open the site without any server. HTML URLs, if not downloaded locally, will be directed to their original source online.
- Open the site with a server -- manual: assets will be downloaded once requested and once the prompt is confirmed.
- Open the site with a server -- auto: a level 1 recursion will be set as each site is visited. A config can be provided to disallow certain files from downloading, or only be limited to a defined set of files.

## Motiviation

I want to use websites offline. Is this too much to ask?
