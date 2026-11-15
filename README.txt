WOCOM GLOBAL: WEBSITE PACKAGE
=============================
wocomglobal.org  |  Word Communication Ministries / Christ Family Assembly, Ibadan

WHAT IS IN THIS FOLDER
----------------------
index.html                       The entire website, one self contained file.
                                 All 10 pages, all photography, the logo and all
                                 styling are inside it. No build step, no server.
banners/social/                  5 social media graphics, exact platform sizes.
banners/page-headers/            9 sub page header banners (1920 x 600).

HOW TO PUT IT ONLINE
--------------------
1. Upload index.html to the root of your hosting (cPanel File Manager, Netlify
   drag and drop, Vercel, GitHub Pages, Cloudflare Pages).
2. Nothing else needs uploading. The banners folder is for social media and
   print, not required by the site.
3. Point wocomglobal.org at the host and enable free HTTPS.

PAGES
-----
#/              Home (hero, service times, upcoming events, welcome, pastors,
                EMPOWER values, departments, Unique Woman, missions, branches,
                media, giving, map, first visit)
#/about         About us
#/leadership    Leadership
#/ministries    Ministries + Join a department form
#/missions      Missions and outreach + outreach events + mission team form
#/unique-woman  The Unique Woman
#/branches      Branches (searchable directory of all 12 assemblies)
#/media         Media / Realities Broadcast
#/events        Events + Upcoming events grid + event alerts form
#/give          Giving (all five accounts, tap to copy)
#/visit         Plan a visit (map + welcome form)

FORMS AND WHERE THEY GO
-----------------------
There are four forms, all posting to one email address:
  Plan a visit                  (visit page)
  Join a department             (ministries page)
  Event alerts signup           (events page)
  Missions team interest        (missions page)
Every form collects name, email address and phone or WhatsApp number, plus the
details relevant to that form.

TO SET THE DESTINATION EMAIL
----------------------------
Open index.html in a text editor and find this line near the bottom:

  var FORM_EMAIL = 'info@wocomglobal.org';

Replace that address with the church office inbox, for example
office@wocomglobal.org, and save.

The forms send through FormSubmit, which needs no account and no server.

IMPORTANT: FormSubmit activation
The first time a form is submitted, FormSubmit sends a one time confirmation
email to the address above. Open that email and click the activation link once.
After that every submission is delivered normally. If an address is never
activated, visitors see a fallback message with a direct email link, so nothing
is lost. This is why the placeholder address must be replaced before launch.

EDITING EVENTS
--------------
Two lists near the top of the script block control both event sections:

  var EVENTS    = [...]   upcoming events (home page shows the first three)
  var OUTREACH  = [...]   outreach events on the missions page

Each entry takes tag, when, title, where, note, link and linkLabel. Add, remove
or reorder entries and the page updates. Keep the file saved and re-upload.

DESIGN NOTES
------------
Palette: navy #143475 (from the logo), gold #C9A24B, cream #F9F4EA.
Type: Fraunces (display) and Manrope (text), loaded from Google Fonts.
No em dashes or en dashes are used anywhere in the site copy.

BEFORE YOU GO LIVE
------------------
1. Replace the FORM_EMAIL placeholder and activate FormSubmit.
2. Kelvin Olorunnisola's title reads "Minister, WOCOM Centre" because the Drive
   folder had his portrait but no role. Confirm or correct it.
3. Media page: broadcast times, sermon library and daily devotional are marked
   as being published. Replace with the real schedule.
4. Event and outreach dates are set to "dates to be announced" because they were
   not supplied. Update the two arrays above as dates are confirmed.
5. Footer Privacy and Beliefs links point to the About page. Supply real pages.
6. Confirm service times (Sunday 9:00 AM, Tuesday 5:00 PM) and the office phone
   (+234 803 380 3905).

CONTENT SOURCES
---------------
Copy and data come from the supplied Drive folder: "CFA - What We Are About",
"Senior Pastors Profile", "Giving Details", "CFA Pastors" (12 branches) and the
WOCOM photography and logo files.

MOBILE BEHAVIOUR (changed this round)
------------------------------------
1. The menu opens as a panel anchored to the RIGHT edge of the screen, covering
   about 88 percent of the width, with the page dimmed behind it. The close X is
   at the top of the panel. Tapping the dimmed area also closes it.
2. Leadership page: on phones each lead pastor portrait sits above the text at
   full width, and the long biography is shortened with a READ MORE button that
   expands it in place (READ LESS closes it again). On desktop both bios show in
   full and no button appears.
3. Lead pastor portraits are now square, the same shape and size as the resident
   pastor portraits further down the Leadership page.
4. Footer on phones shows only the brand block and the JOIN US column with
   service times, address and phone. The Church, Next Steps and Media link
   columns are hidden on phones and still show on desktop and tablet.
