# Dave Mishal — Nordstrom.com Holiday Growth Landing Page

This folder is ready for static hosting on GitHub Pages or Cloudflare Pages.

## Files
- `index.html` — complete landing page
- `assets/hero-holiday.webp`
- `assets/sponsored-banner.webp`
- `assets/editorial-placement.webp`
- `assets/strategy-lifestyle.webp`
- `assets/dave.webp`

## Recommended free setup

### 1. Host the landing page on GitHub Pages
1. Create a new public GitHub repository.
2. Upload `index.html` and the `assets` folder to the repository root.
3. Open the repository **Settings**.
4. Open **Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/ (root)`.
7. Save.
8. GitHub will provide a public `github.io` URL.

You can later connect a custom domain if you own one.

### 2. Create the Google Calendar Appointment Schedule
On a computer, open Google Calendar and create an **Appointment schedule** with:

- Title: `Nordstrom Growth Review`
- Duration: `20 minutes`
- Availability: Monday–Friday, 9:00 AM–5:00 PM
- Time zone: America/Los_Angeles
- Buffer time: 10 minutes
- Conferencing: Google Meet
- Check calendars for availability: ON
- Form fields:
  - First name
  - Last name
  - Email
  - Brand / Company
  - Website (optional)
- Suggested booking window: 21 days
- Suggested minimum lead time: 2 hours

Google's booking page automatically removes times when your checked calendar is busy.

### 3. Embed the booking page in `index.html`
In Google Calendar:
1. Under **Booking pages**, open the three-dot menu for the schedule.
2. Choose **Sharing options**.
3. Choose **Website embed**.
4. Choose **A single booking page**.
5. Choose **Inline booking page**.
6. Copy the code.

In `index.html`, find:

`PASTE GOOGLE INLINE BOOKING EMBED HERE`

Delete the placeholder `<div class="calendar-placeholder" ...>...</div>` and paste Google's embed code inside:

`<div class="calendar-shell" id="google-calendar-booking"> ... </div>`

Save and push the updated `index.html` to GitHub. GitHub Pages will redeploy automatically.

## Why this setup
The website stays static and free to host, while Google Calendar handles live availability, conflict blocking, booking confirmations, and Google Meet creation.

## Notes
- The sponsored placements on the page are illustrative mockups.
- The page does not use the Nordstrom logo or imply Nordstrom affiliation.
- Replace `assets/dave.webp` with Dave's full-resolution LinkedIn profile photo when available for the best visual quality.
