# Brand Academy pilot landing page

Static, responsive single-file page for the existing GitHub Pages registration URL. Reuses the approved local pilot welcome design and the existing Formspree endpoint. No build step or new subscription.

## Existing destinations
- Repository: https://github.com/NearFarAdvisory/spurcorpacademy
- Registration: https://nearfaradvisory.github.io/spurcorpacademy/
- Form POST: https://formspree.io/f/mvkpqweb
- Thinkific: https://brand-academy-s-site.thinkific.com/users/sign_in?redirect_to=%2Fhub

## Form compatibility
Preserves full-name, email, contact-number, agency-status, agency-name-new, agency-name-existing, brands (repeated), stores, additional-notes and _gotcha. Adds source, cohort and registration-purpose. Preserves all existing agency and brand choices. Removes the obsolete Netlify redirect and disconnected validation code. JavaScript enforces active agency and at least one brand, prevents concurrent/repeated successful submits, retains data on failure, and acknowledges only successful HTTP responses. Without JavaScript the native Formspree submission path remains available, but conditional and group validation are limited.

No personal information is stored in GitHub, URLs or browser local storage by this page. Formspree account controls, retention, notification recipients and actual delivery require verification by its owner. Frontend validation is not a security boundary.

## Publish
Replace root index.html on main. Confirm existing Pages source before altering deployment settings; docs/CNAME was preserved. Verify the public page after deployment. No Thinkific settings are changed.

## Process
Landing page → Formspree receipt → registration review and brand/store mapping → confirmed Thinkific invitation/enrolment → self-paced orientation and learning → pilot feedback.

The landing page implements the registration step. It does not provision accounts or promise immediate access. See the local process handover for proposed internal communications and automation; these are not activated by this website.
