# Lead Analytics Setup

The portfolio is ready for lead-intent tracking through `data-lead-event` attributes on high-value links such as CV downloads, Calendly, email, LinkedIn, GitHub, YouTube and video intro.

## Important boundary

Analytics can show visits, referrers, locations in aggregate, device type and click events. It cannot give visitor names or email addresses unless the visitor voluntarily shares contact details through a form, Calendly booking, email or newsletter signup.

For Germany/EU visitors, collect personal contact data only with clear consent and a privacy notice.

## Recommended setup

1. Privacy-friendly analytics:
   - Plausible, Simple Analytics or Umami for aggregate page and click analytics.
   - Google Analytics only if you also add a cookie/consent banner and privacy policy wording.

2. Lead capture:
   - Calendly is already embedded and collects contact details from booked calls.
   - Add a form service such as Tally, Basin, Formspree or Netlify Forms if you want visitors to request a call or send a project inquiry directly from the page.

3. Event tracking:
   - The page includes a small `trackLeadEvent()` helper.
   - If Google Analytics `gtag` is added later, link clicks will automatically emit events under category `lead_intent`.

## Current lead-intent events

- `hero_resume_click`
- `hero_video_click`
- `work_resume_click`
- `video_intro_click`
- `youtube_click`
- `english_cv_click`
- `german_cv_click`
- `calendly_click`
- `email_click`
- `linkedin_click`
- `github_click`
- `youtube_footer_click`
- `footer_email_click`
- `footer_linkedin_click`
- `footer_github_click`
- `footer_youtube_click`

