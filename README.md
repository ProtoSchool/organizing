# Organizing

Organizing a ProtoSchool chapter? Wish you were? Start here!
___

Whether you're an existing organizer or hope to become one, please read and abide by our [Code of Conduct](https://github.com/ipfs/community/blob/master/code-of-conduct.md).

___

## How to start a new ProtoSchool chapter

After reviewing our [Code of Conduct](https://github.com/ipfs/community/blob/master/code-of-conduct.md), please [open an issue](`https://github.com/protoschool/organizing/issues/new?labels=new-chapter&title=New%20Chapter%20Request&body=Please%20introduce%20yourself%20and%20tell%20us%20where%20you'd%20like%20to%20host%20a%20ProtoSchool%20chapter.`) on this repo asking to be added as a chapter organizer. This is an opportunity to introduce yourself and why you're interested in organizing. Here's an example to get you started:

>Hi, I would like to start a ProtoSchool chapter for [name of geographic community]. I am [@YourTwitterName] on twitter and work at/on [project/organization]. I will be co-organizing this chapter with [names of other organizers]. I have been using [IPFS/IPLD/LibP2P/Multi-Format] for X months and would like to help others learn as well.

Be sure to send us your requested chapter name, which must be short and all lower case. It should ideally be the name of the city where your workshops will be held, or alternatively an area that's small yet meaningful. Choose `boston` or `metrowest` instead of `massachusetts` or `usa`.

An existing owner will need to respond and create your chapter repository for you.

Once you are an organizer, follow these instructions to set up the web presence for your ProtoSchool chapter:

**Step 1** | You should have been added to the team called chapter-organizers and should have access to edit the new chapter repo, e.g. https://github.com/protoschool/boston

**Step 2**
Each chapter can set up their own `gh-pages` branch on their org GitHub pages will automatically route http://proto.school/<reponame> to it.

**Step 3** | You should create a Code of Conduct for your website and repository. You can use this template as a starting point. Be sure to make all people feel welcome at your event.


**Step 4** | _This step is important for discoverability!_

Once your chapter is up and running, make a pull request to the ProtoSchool website to add a chapter JSON file to the `/chapters` directory. When your request is accepted, your chapter will get auto-added to the listings at http://proto.school/chapters.html

Your chapter JSON file should look something like this:

```
{
  "name": "Boston NodeSchool",
  "location": "Boston MA",
  "country": "US",
  "region": "North America",
  "organizers": ["terichadbourne"],
  "website": "http://proto.school/boston",
  "twitter": "bostonprotoschool",
  "repo": "http://github.com/protoschool/boston"
}
```
Please be sure to format your JSON data according to the following guidelines. (Fields marked in bold are required.)

| Field | Description |
| --- | --- |
| **name** | Whatever you call your events, often <location> ProtoSchool |
| **location**	 | This appears on the chapters.html page, often <City> or <City, State> but can be any geocode-able string |
| country	 |  If your location isn't itself a country, use this field to list the ISO-3166 2-letter country code for consistency |
| **region**  |  Choose an existing region from the chapters page if possible--if not then pick a broad, non-country region name |
| organizers  | An array of GitHub usernames  |
| website  |  URL of the main website for your chapter, if one exists besides your GitHub repo |
| **repo** |  GitHub repo URL |
| other   | Any other services like Twitter, Gitter, etc. that exist for the chapter (not the organizer's info)  |


## Why we take this approach to chapter setup
- Chapters get their own website.
- We can easily list all of the chapters on the ProtoSchool site.
- Chapters get their own "mailing list" in the form of GitHub issues. These can be in other languages as well, e.g. Spanish for Latin-American Chapters, whereas the main repos are primarily in English.
- All ProtoSchool event attendees leave with a GitHub account and a community of whom they can ask questions.
- Since all chapter members are [open open source](https://github.com/Level/community/blob/master/CONTRIBUTING.md) style contributors, everyone is empowered to help moderate discussions and improve the chapter website.
