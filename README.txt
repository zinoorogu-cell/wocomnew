WOCOM GLOBAL: WEBSITE PACKAGE
=============================
wocomglobal.org  |  Word Communication Ministries / Christ Family Assembly, Ibadan

WHAT IS IN THIS FOLDER
----------------------
index.html                       The website: all 10 pages, styling and script.
images/                          Every photo and the logo as separate files, named
                                 with their exact pixel size. See IMAGE-GUIDE.txt.
IMAGE-GUIDE.txt                  How to swap any image, plus the full file list.
banners/social/                  5 social media graphics, exact platform sizes.
banners/page-headers/            9 sub page header banners (1920 x 600).

HOW TO PUT IT ONLINE
--------------------
1. Upload index.html AND the images folder to the root of your hosting (cPanel
   File Manager, Netlify drag and drop, Vercel, GitHub Pages, Cloudflare Pages).
2. The banners folder is for social media and print, not required by the site.
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

BANNERS (latest round)
----------------------
All ten page header banners were replaced with new photographs and the
"Choir & Worship" card on the Ministries page now shows the choir in blue and
navy. The leadership banner changed from .png to .jpg, and its path in
index.html was updated. See IMAGE-GUIDE.txt for the photo used on each page.

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

UPDATES THIS ROUND (editor feedback from Hassan)
------------------------------------------------
1. Instagram corrected to @wocomworld, https://www.instagram.com/wocomworld
   (the earlier @wocomworldcfa handle was wrong). Used in the media page, the
   footer and the Life at WOCOM section.
2. Founding year is now 1985 throughout (hero, About page, footer, counters).
   Christ Family Assembly remains the church arm that began in 1990.
3. Pastor Kelvin Olorunnisola is listed as National Overseer, Word
   Communication Ministries.
4. Apostle Sunday A. Popoola is listed as President and Set Man.
5. London branch phone number is +44 203 649 8947 (tap to call works).
6. Events that fall in the next year now read 2027: Power of Faith Convention
   (August 2027), The Unique Woman Conference, Bone of My Bone Seminar, Roots
   Outreach Camp, City-wide Crusade, ICOM intake and the Unique Woman community
   outreach. Edit the EVENTS and OUTREACH arrays to update them.
7. Home page rebalanced away from leaders: the large pastor section is replaced
   by a compact leadership strip with small portraits and counters, and new
   sections were added that lead with church life instead:
   Life at WOCOM photo wall, a rotating quote carousel, Find your people (eight
   icon cards), a Next Steps row and a prayer request form. Full leader profiles
   live on the Leadership page only.
8. Icons added across the site (service times, section labels, next steps, the
   Find your people cards, giving, branches, maps, media).
9. Motion added for a younger feel: floating gradient orbs in the hero, animated
   counters, an auto rotating quote carousel, gentle photo tilt on hover, light
   parallax on the photo wall, hover lifts on cards, and the existing ticker.
   All of it respects the visitor's reduced motion setting.

NEW FORM
--------
Send a prayer request (home page, Next Steps block). It posts to the same
FORM_EMAIL address as the other four forms.

LIFE AT WOCOM AND THE FEED (this round)
---------------------------------------
The home page now uses the church's own Facebook and Instagram captions, taken
from the public WOCOM page (facebook.com/wocomchurch):
  - Photo wall captions quote the page, for example "Moments of worship, the
    power of the Word, and hearts united in His presence", "No matter how your
    week has been, there is room for you in God's presence", "Sunday fits, good
    vibes and kingdom energy".
  - The rotating quote card cycles five lines from the page.
  - A new "Straight from our feed" grid shows four recent posts with a short
    summary and a link out to the original post or video. Two posts were removed
    on request: the humorous "bank balance" post and the "content guy" post.

Captions were pulled from public search results for the page, because Facebook
blocks automated reading of its pages. If any line should be reworded, edit it
in 2_home.html (the block marked LIFE AT WOCOM and STRAIGHT FROM OUR FEED).
New posts can be added by copying one feed-card article and changing the text,
the tag and the link.

BRANCH PHONE NUMBERS (privacy)
------------------------------
Branch numbers are no longer printed anywhere in the page. Each branch card now
shows a "Contact this branch" button, and only when a visitor taps it does the
card reveal a Call link and a WhatsApp link. The numbers are stored encoded in
the script and decoded in the browser at that moment, so a scraper reading the
HTML finds no branch numbers and no tel: links for branches.

What this does and does not do: the numbers cannot be harvested from the page
source by ordinary scrapers, which is what was asked. It is not absolute
protection, because a determined person running the page in a browser can still
read a number after clicking. For real protection, route calls through a
contact form or a call-tracking service instead of a direct line.

The office number on the top bar, the visit page and the footer is still shown
plainly. Say the word and the same click to reveal treatment can be applied
there too.

ANIMATED HOME BANNER TEXT
-------------------------
The hero headline, badge, sub text, buttons and service details now animate in
one word or element at a time when the page loads. The gold italic phrase also
has a slow shimmer sweep. It is pure CSS plus a small word splitter, so the text
still shows in full if JavaScript is off, and it switches itself off for
visitors who have reduced motion turned on.
