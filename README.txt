SYLVIA MWIHAKI · PORTFOLIO WEBSITE (ready to go live)
=====================================================

WHAT'S IN THIS FOLDER
  index.html                         the whole site
  img/  fonts/  js/                  images, fonts and the two small code libraries
  Sylvia_Mwihaki_Portfolio_2026.pdf  the PDF portfolio (linked from the site)
  favicon.png, apple-touch-icon.png  browser tab and phone home-screen icons
  og.jpg                             the preview picture shown when the link is shared

Everything is self-contained. The site makes no requests to Google or any other
third party (fonts and code are hosted in this folder), so no cookie banner is needed.

PUT IT ONLINE WITH VERCEL (free)
  1. Go to vercel.com and sign up (Continue with GitHub or email).
  2. Add New... > Project > deploy this folder:
       - Easiest: install the Vercel CLI, open a terminal in this folder and run:  npx vercel
         Answer the questions (all defaults are fine). Then run:  npx vercel --prod
       - Or put the folder in a GitHub repository and import that repository in Vercel.
  3. Your site is live on a *.vercel.app address.

USE YOUR OWN DOMAIN
  In Vercel: Project > Settings > Domains > add your domain (for example sylviamwihaki.com)
  and follow the DNS steps it shows for your domain registrar.

AFTER THE DOMAIN IS LIVE (1 small edit)
  Link previews (WhatsApp, LinkedIn, Slack) need a full web address for the preview picture.
  In index.html, change   content="og.jpg"   to   content="https://YOUR-DOMAIN/og.jpg"

THE LOCATION-AWARE TOUCHES
  The site reads the visitor's device time zone and language (no pop-up, nothing stored).
  - Visitors in Kenya see the home version (Sheng first).
  - Everyone else gets English first, a hello in their language next to "Sasa!",
    their city on the matatu route (NAIROBI -> BERLIN), a second clock in the menu,
    and "Alight in [city]" at the end of the ride.
  - The city comes from the time zone, so someone in Munich sees Berlin, and anyone
    in the UK sees London.
  Preview any city by adding this to the address:   ?tz=Europe/Lisbon&hl=pt
  (other examples: ?tz=Europe/Berlin&hl=de   ?tz=Europe/Amsterdam&hl=nl   ?tz=Europe/London)
