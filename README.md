# Organizing

Organizing a ProtoSchool chapter? Wish you were? You're in the right place!

_For more background on ProtoSchool or other ways to get involved, like building workshops, check out our [guide to contributing](https://github.com/protoschool/organizing/blob/master/CONTRIBUTING.md) or view our [launch presentation](https://github.com/protoschool/organizing/blob/master/presentations/ProtoSchool_Launch_Preso_2019-01-14.pdf)._

## How to start a new ProtoSchool chapter

Whether you're an existing organizer or hope to become one, please read our [Code of Conduct](https://github.com/protoschool/organizing/blob/master/CODE_OF_CONDUCT.md). All chapter organizers are expected to follow these guidelines to ensure the ProtoSchool community remains a welcoming place for all learners.

Check out our [list of existing chapters](https://proto.school/#/chapters) to see if there's already a group near you. If not, please [open an issue](https://github.com/ProtoSchool/organizing/issues/new?assignees=terichadbourne&labels=new-chapter&template=new-chapter-request.md&title=New+Chapter+Request+-+%5BLocation%5D) on this repo asking to be added as a chapter organizer. This is an opportunity to introduce yourself and why you're interested in organizing. Here's an example to get you started:

>Hi, I would like to start a ProtoSchool chapter for [name of geographic community]. I am [@YourTwitterName] on twitter and work at/on [project/organization]. I will be co-organizing this chapter with [names of other organizers]. I have been using [IPFS/IPLD/libPp2p/Multiformats] for X months and would like to help others learn as well.

Be sure to send us your requested chapter name, which must be short and all lower case. It should ideally be the name of the city where your workshops will be held. Choose `san-francisco` instead of `bay-area`, `california` or `usa`.

As a chapter organizer, you'll be responsible making all members feel welcome, which means upholding and enforcing your chapter's own Code of Conduct. You'll need to supply contact information that can be used by members to report and violations of that CoC within your chapter's repo or events.

Once you submit your request, a maintainer will respond with any questions and will then help to set up your chapter repository.

Once you are an organizer, follow these instructions to set up the web presence for your ProtoSchool chapter:

**Step 1** | You should have been added to the team called chapter-organizers and should have access to edit the new chapter repo, e.g. https://github.com/protoschool/san-francisco

**Step 2**

Update your readme to introduce your chapter. Be sure to note who the chapter organizers are, include a link to a website (if you have one), and note where members can find event listings. If you'll be creating a chapter website (see below), it's fine to keep the readme brief and link there for more detail.

**Step 3**
Create a Code of Conduct for your website and repository. The [Contributor Covenant](https://www.contributor-covenant.org/) provides a nice template.

You should also create a Code of Conduct for your events, as part of the broader effort
to make all people feel welcome. The [Conference Code of Conduct](http://confcodeofconduct.com/)
provides a nice starting point, but will require some adaptation to the specifics
of your events.

In any Code of Conduct you create, be sure to **include contact information and a procedure for
reporting any incidents to chapter leadership**.

**Step 4 (Optional)**
Each chapter can set up their own `gh-pages` branch on their org and [GitHub Pages](https://help.github.com/categories/github-pages-basics/) will automatically route http://proto.school/<reponame> to it.

(If you prefer to build a website on another platform or use a Meetup page as your website, that's fine, you just won't be able to host it on our domain.)


**Step 5** | _This step is important for discoverability!_

Once your chapter is up and running, make a pull request to the ProtoSchool website
to add you chapter to the existing `chapters.json` file in the `/chapters` directory.
When your pull request is accepted, your chapter will be automatically added to the listings at http://proto.school/#/chapters

You may take this step before or without building a chapter website, as long as you've completed the other
steps described above to get your repo set up. Should you decide to build a website later, be sure to create a new PR adding your website URL to your chapter listing so that users will be directed to your website instead of your repo.

Your addition to the `chapters.json` file should look something like this:

```
,
{
  "name": "ProtoSchool San Francisco",
  "city": "San Francisco, CA",
  "country": "US",
  "region": "North America",
  "organizers": ["mikeal"],
  "website": "http://proto.school/san-francisco",
  "twitter": "sfprotoschool",
  "repo": "http://github.com/protoschool/san-francisco"
}
```
Please be sure to format your JSON data according to the following guidelines. (Fields marked in bold are required.)

| Field | Description |
| --- | --- |
| **name** | Whatever you call your events, often "ProtoSchool <City> " |
| **city**	 | The name of your city or town, which will appear on the Chapters page, often <City> or <City, State> but can be any geocode-able string |
| **country**	 |  Please list your country's [ISO-3166 2-letter country code](https://en.wikipedia.org/wiki/ISO_3166-2) for consistency |
| **region**  |  Choose an existing region from the chapters page if possible--if not then pick a broad, non-country region name |
| organizers  | An array of GitHub usernames  |
| website  |  URL of the main website for your chapter, if one exists besides your GitHub repo |
| **repo** |  GitHub repo URL (if no website field exists, your chapter listing will direct to this URL)|
| other   | Any other services like Twitter, Gitter, etc. that exist for the chapter (not the organizer's info)  |


## Why we take this approach to chapter setup
- Chapters get their own website at http://proto.school/chapter-name" if they push to a `gh-pages` branch.
- We can easily list all of the chapters on the ProtoSchool website.
- Chapters get their own "mailing list" in the form of GitHub issues. These can be in other languages as well (e.g. Spanish for Latin American chapters), whereas the main repos are primarily in English.
- All ProtoSchool event attendees leave with a GitHub account and a community of whom they can ask questions.
- Since all chapter members are [open open source](https://github.com/Level/community/blob/master/CONTRIBUTING.md) style contributors, everyone is empowered to help moderate discussions and improve the chapter website.
