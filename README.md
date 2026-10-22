# Protocol Personal Health public information

Static homepage and privacy policy for the privately operated Protocol tracker
and its Google Health OAuth consent configuration. This repository contains only
public descriptive content. Do not add application source, personal records,
reports, runtime data, internal network addresses, credentials, or tokens.

The private tracker and connector are separate repositories and installations.
Changing or publishing this site does not modify or restart either application.

## Local preview

From this directory, run `python3 -m http.server 8081 --bind 127.0.0.1` and open
`http://127.0.0.1:8081/`. Stop that exact preview process when finished.
There are no dependencies, JavaScript, build step, remote fonts, or analytics.

## Hosting

GitHub Free, in the separate public repository `NICKOGALLC/protocol-public-site`.
GitHub Pages is enabled with `main` and `/` as its source, with HTTPS enforced. Retain
`.nojekyll` so the pages are served as plain static files. A paid plan or custom
domain is unnecessary for hosting. This does not guarantee Google's acceptance
of the OAuth branding URLs; that must be checked in the actual Cloud project.

Published addresses (verified over HTTPS on 2026-10-21):

- Homepage: `https://nickogallc.github.io/protocol-public-site/`
- Privacy: `https://nickogallc.github.io/protocol-public-site/privacy.html`
- Authorized domain to try: `nickogallc.github.io` (not the entire `github.io`
  provider domain and not a URL with a scheme or path).

Keep the existing Google OAuth redirect URI and read-only scopes unchanged.
If Google requires domain ownership verification, use Search Console with the
account associated with the Cloud project and its supported URL-prefix HTML-tag
or HTML-file method for the hosted site. Do not claim ownership of `github.io`.
Do not purchase a domain, enable billing, alter network access, or switch APIs
to bypass a rejection. Record the exact non-secret validation message instead.

After Google actually reports **In production**, explicitly reauthorize the
existing connector, verify one token renewal and a bounded read, and check the
app's saved collection status. Neither publishing this site nor one successful
refresh proves indefinite authorization.

## Content maintenance

Match the consent-screen application name, currently **Protocol Personal Health**.
Review the policy against the private application's actual data handling when
that behavior changes; do not promise deletion controls or retention behavior
that the application does not implement. The effective date is in `privacy.html`.
Public repository issues are for non-sensitive contact only.

## Initial verification

On 2026-10-21, the homepage, privacy page, and stylesheet returned HTTP 200
from an isolated loopback preview. HTML structure, unique IDs, and all 14 local
links/anchors passed checks. Chromium desktop (1440 px) and mobile (390 px)
renders were inspected. The six publication files contain no application
source, health records, credentials, or internal deployment addresses.
GitHub reported a successful Pages build of `bd6ea0f`. The three public page/CSS
responses returned HTTP 200 and matched the reviewed local files byte for byte.
The owner subsequently supplied a Console screenshot showing **In production**
and **Back to testing** after entering the site information. The separate
verification banner remains; personal-use verification exceptions do not imply
that Google has verified the application. The existing private connector was
then reauthorized; forced renewal, a bounded read, and verification of the same
three read-only permissions passed. The saved history import resumed with
automatic collection enabled. This verifies current access, not indefinite
token validity. No tracker service restart or data migration was needed.

Before publication, inspect every staged file and the entire history for private
content. Validate local links, semantic HTML, keyboard navigation, narrow-screen
layout, and HTTP responses. Publishing or updating GitHub requires the owner's
authorization and the owning workstation's execution workflow.
