# Task 2: Improve the matching algorithm

This task is closely related to [Task 3: add other LLMs to Harmony](./3-add-llms.md)

## Related issues:

* https://github.com/harmonydata/app/issues/14
* https://github.com/harmonydata/app/issues/15
* https://github.com/harmonydata/harmonyapi/issues/4
* https://github.com/harmonydata/harmony/issues/22
  
Harmony often matches items that should not be matched, or vice versa, e.g.

*Feeling tired or having little energy?* was incorrectly matched to *Having upsetting dreams that replay part of the experience or are clearly related to the experience?*

We have a Github repo where we have experimented with this: https://github.com/harmonydata/matching 

So how can we improve the matching? 

* Probably the easiest way would be to switch this underlying model, rather than trying anything clever. See also [Task 3: add other LLMs to Harmony](./3-add-llms.md)
* Longer term an LLM could be fine-tuned but that needs lots of resources and lots of data!


## Explicit user feedback on the web UI

You will notice that on the web UI there are options for users to tag a harmonisation as incorrect.

We store this data. I exported it on 18 April 2024. Maybe we can use this data to improve the tool?

All saved harmonisations

https://harmonyapistorage.z33.web.core.windows.net/harmonisations.json

All mismatches tagged by users in the web UI:

https://harmonyapistorage.z33.web.core.windows.net/mismatches.json

All user ratings:

https://harmonyapistorage.z33.web.core.windows.net/ratings.json
