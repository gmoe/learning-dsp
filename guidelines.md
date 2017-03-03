---
layout: default
title: Submission Guidelines
---

Resource links can be found inside the `_data` directory of this repository,
inside of JSON files specific to each topic. All of the JSON files are listed
in the `_data/index.json` files.

# Adding a New Topic

Topic files are single JSON objects that have two properties:

* **sectionName** - The name of the topic (i.e. *Physical Modeling*)
* **links** - An array of resource entry objects

Once you have created the topic object, add it to the index file so that it can
be processed by Jekyll. The index file contains an array of file names for each
topic JSON file, omitting the file extension.

# Adding Resource Entries

A resource entry is stored as a JSON object with three properties:

* **title** - The display name of the resource (i.e. *"Doppler Simulation and
  the Leslie*")
* **type** - What kind of content the resource is (i.e. `"document"`)
* **link** - The URL to the resource

The `type` property affects which icon gets prepended to the entry in the list.
Currently this website supports `book` and `video` for online textbooks and
video resources respectively.  An example of this type of JSON object can be
found below:

```
{
  "title": "Doppler Simulation and the Leslie",
  "type": "document",
  "link": "https://ccrma.stanford.edu/~jos/doppler/doppler.pdf"
}
```
