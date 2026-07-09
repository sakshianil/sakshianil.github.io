# Lead Analytics Setup

The portfolio is ready for lead-intent tracking through `data-lead-event` attributes on high-value links such as CV downloads, Calendly, email, LinkedIn, GitHub, YouTube and video intro.

## Implemented (live)

1. **Privacy-friendly analytics**
   - Plausible (`script.tagged-events.js`) with domain `sakshianil.github.io`
   - Custom goals via `trackLeadEvent()` — works with Plausible tagged events and optional Google Analytics `gtag`

2. **Lead capture**
   - Calendly embedded in the meeting section
   - GDPR consent inquiry form (FormSubmit → `sbbinfo90@gmail.com`) in `#inquiry`
   - Privacy notice in footer (EN/DE)

3. **Event tracking**
   - `trackLeadEvent()` emits to Plausible and/or GA when configured

## Important boundary

Analytics can show visits, referrers, locations in aggregate, device type and click events. It cannot give visitor names or email addresses unless the visitor voluntarily shares contact details through a form, Calendly booking, email or newsletter signup.

For Germany/EU visitors, collect personal contact data only with clear consent and a privacy notice.

## Recommended setup

1. **Plausible dashboard**: register `sakshianil.github.io` at [plausible.io](https://plausible.io) and map custom events to goals (all `data-lead-event` names below).

2. **FormSubmit**: confirm the first submission email from FormSubmit to activate the inquiry form.

3. **Optional**: swap FormSubmit for Tally, Basin, Formspree or Netlify Forms if you prefer a managed inbox UI.

## Current lead-intent events

- `hero_resume_click`
- `hero_video_click`
- `inspire_youtube_click`
- `work_resume_click`
- `video_intro_click`
- `youtube_click`
- `english_cv_click`
- `german_cv_click`
- `calendly_click`
- `inquiry_submit`
- `email_click`
- `linkedin_click`
- `github_click`
- `youtube_footer_click`
- `footer_email_click`
- `footer_linkedin_click`
- `footer_github_click`
- `footer_youtube_click`

