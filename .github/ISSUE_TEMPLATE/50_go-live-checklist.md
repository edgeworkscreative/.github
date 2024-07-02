---
name:  ✔ GO-LIVE Checklist
about: A checklist of things to be done for a site to go live.
title: 'GO-LIVE Checklist'
labels: ['info']
assignees: ''
---

# Site-Ready Checklist

Make sure the following items have been checked to confirm the website is ready for launch.

## On-Site Items

* [ ] Does the website render match the XD design or other directive/expectation?
* [ ] Does the contact form work?
* [ ] Do other forms on the site work?
* [ ] Do we have a 301.csv prepared? (if redeisgn)
* [ ] Do any form functions such as trigerring emails perform as expected?
* [ ] Do we have the correct contacts, email addresses, social media links, business address, etc. ready for the .env file for the live server?
* [ ] Do important pages have titles, keywords, and meta descriptions?
* [ ] Are there garbage test data records? If so, nuke em
* [ ] Are links in header naviagtion working?
* [ ] Are links in footer or sidebar navigation working?
* [ ] Are policy pages (privacy, accessibility, terms of use) needed and prepared?
* [ ] Does the site have a favicon?
* [ ] Does the site have a default Page OG image prepared?
* [ ] Does the site use default blog featured images?
* [ ] Are appropriate User Accounts configured?
* [ ] Have other admin logins been tested? Avoid training nightmares because users don't have the permissions they need.
* [ ] Is the 404 page configured and does it look good?
* [ ] Are images using ALT text?
* [ ] Do you have a complete zip of /uploads for the live server?
* [ ] Are page semantics in place? (h1-h2-etc)
* [ ] Are there any new modules on this site which need Help Files? 
* [ ] Are there console errors? Can they be resolved?
* [ ] Are there other console messages we can eliminate? Is there debug messaging that can be removed?

## Lighthouse, Page Speed and Mobile Testing

Run Lighthouse in the browser on exmaple pages for all major templates.

Sample pages will ideally have passing scores for Accessibility (ACC), Performance(PER), and SEO. If you identify a fix that directly improves a score and it is an Edgeworks CMS update and not client-specific, please add your update to the main [Edgeworks CMS repo](https://github.com/edgeworkscreative/Edgeworks-CMS) so we benefit downstream.

Please record scores from Lighthouse tests below in the format Desktop / Mobile  (e.g. 88/92) and confirm mobile testing for responsive usability (RESP) with a X or other indicator. Page Speed score can be obtained from [Page Speed Insights](https://pagespeed.web.dev/https:/)



| Template | Page URL | ACC | PER | SEO | RESP | SPEED |
| ---------- | ---------- | ----- | ----- | ----- | ------ | ------- |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |
|          |          |     |     |     |      |       |


## Go-Live

Make sure the following happens:

* [ ] Live database is created with new user / credentails limited to that domain
* [ ] Live Plesk domain is created
* [ ] Connect the domain to GitHub repo master branch
* [ ] Remember to RDP into the server to run composer
* [ ] If the project is one which is using GitFlow (master / dev / release) the Plesk can be set to automatically pull from the repo. If the project only has a master branch ***do not pull automatically *** - we want the human interface/decision to push updates to the live server.
* [ ] You may need to manage Plesk and GitHub keys - have fun with that.
* [ ] Configure .env for live
* [ ] Set up or confirm Cloudflare account exists
* [ ] Change any DNS as needed for the go-live
* [ ] transfer /uploads and make sure all expected /uploads/__FOLDERS exist
* [ ] test all main forms once site is live - confirm all expected actions take place [see below]
* [ ] Is the site using any third party integrations that require keys, accounts or other settings for the live site?
* [ ] Will the site require any CRON jobs?
* [ ] Once site is up go to admin settings to auto-gen robots, links, etc
* [ ] Once site is up run any Publish mechanisms (e.g. Nav, CMS posts)
* [ ] Any Cloudflare Page Rules or cache setups? Always HTTPS etc

### Website Forms

After the site has gone live front-end forms and functions must be tested to confirm they work in the live environment. In most cases we are testing a front-end submission process, a notification (email), and logic on the back end for record management and/or admin handling (e.g. accept/deny)

| Form or Function | Page URL | Front End | Notification | Back End |
| ---------- | ---------- | ----- | ----- | ----- |
|     contact form     |          |     |     |     |
|          |          |     |     |     |
|          |          |     |     |     |
|          |          |     |     |     |

### Some very likely third-party things:

* [ ] Google ReCaptcha
* [ ] Google Search Console - claim the site and submit sitemap
* [ ] Google Tag Manager
* [ ] Google Analytics
* [ ] Create Admin report from Looker Studio
* [ ] Accessi.be snippet

## Post-Launch

* [ ] Capture site launch date
* [ ] Schedule training
* [ ] Capture 90-Day Support from date of training
* [ ] Create Hosting recurring invoice

