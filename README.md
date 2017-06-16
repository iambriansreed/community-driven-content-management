# Community Driven Content Management
 
Many times when I want to learn something new or become an expert in a particular technology stack I volunteer my time to build software using that technology. In 2016 I volunteered to build the website for Revolution Conference. I chose to use WordPress as a backend and Angular as a front end. 
 
I was very comfortable in WordPress but wanted to stretch my understanding of Angular. The event attendees and volunteers were happy with the site, however I noticed that the site didn’t get updated very often. The website had lots of content. Speakers, volunteers, and sponsors would ask for updates and the content editors, usually the already overtaxed organizers, would then update the site when they got a free moment. 

## Content Entry Choke Point

That choke point of content entry is a pattern well established in the history of CMSs. For most applications and websites it’s not a big deal. When you have data on 50 different people, giving 50 different talks and the updates are very time sensitive the choke point it much more obvious.
 
The next Revolution Conference rolled around and I decided I would volunteer my time again. I wanted to expand my expertise in Node.js and made that backend decision quickly. I wanted to avoid WordPress and any other traditional CMS altogether. I knew I didn’t want to manage the content in fact I wanted anyone to be able to update the website.
 
## Source Control as a CMS

Eventually the idea of using a web based source control solution as a repository of content dawned on me. Given that Revolution Conf is a conference geared towards professional software developers I knew most of the speakers and attendees worked with Github on a daily basis. Any content I had already added to the website I pulled out and began to structure into a series of JSON, Markdown, images, and directories.
 
Organization of the content just fell into place. Content that didn’t have rich text or images got a single JSON file. More complicated content got a directory for each type then a subdirectory for each item with may contain images, JSON, or markdown. I created a parsing tool which pulls the content down from the Github repo and converts the content into easily consumable data. The process of updating content follows the same path as contributing to an open source project on Github.

## Community Drove the Content

The website was another success and the choke point of content editors was resolved.
We went from 2 or 3 folks updating content to 35 folks consisting of organizers, volunteers and speakers. As designed the community drove the content management on the site. I plan on expanding on this concept and even making a tool for those less code oriented to update content.

The code written for that conversion of content to data has been packaged and released here:
https://www.npmjs.com/package/cdcm
 
You can explore the application repo of the Revolution Conference app here:
https://github.com/RevolutionVA/website2017
 
You can explore the content repo of the Revolution Conference app here:
https://github.com/RevolutionVA/website2017-app
