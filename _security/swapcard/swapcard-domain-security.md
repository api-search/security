---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@swapcard.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swapcard.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:_spf1.swapcard.com include:mail.zendesk.com include:3004554.spf03.hubspotemail.net include:app.outreach.io -all
hosts:
- cert_expires: Aug 21 23:09:20 2026 GMT
  cert_not_before: May 23 22:09:27 2026 GMT
  host: swapcard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 301-redirects to https://www.swapcard.com/
  tls_version: TLSv1.3
- host: developer.swapcard.com
  https: true
  note: 302-redirects to the Swapcard Developer Hub (swapcard.dev). Hosts the live GraphQL endpoints under /event-admin/graphql and /exhibitor/graphql.
- cert_expires: Dec 19 23:59:59 2026 GMT
  cert_not_before: Nov 20 00:00:00 2025 GMT
  host: swapcard.dev
  https: true
  note: Developer documentation hub.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swapcard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swapcard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Swapcard
provider_slug: swapcard
slug: swapcard-domain-security
source_filename: swapcard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + GraphQL endpoint hosts\nhosts:\n- host: swapcard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: May 23 22:09:27 2026 GMT\n  cert_expires: Aug 21 23:09:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 301-redirects to https://www.swapcard.com/\n- host: developer.swapcard.com\n  https: true\n  note: 302-redirects to the Swapcard Developer Hub (swapcard.dev). Hosts the live GraphQL endpoints under /event-admin/graphql and /exhibitor/graphql.\n- host: swapcard.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: Nov 20 00:00:00 2025 GMT\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  note: Developer documentation hub.\nendpoints:\n- url: https://developer.swapcard.com/event-admin/graphql\n  method: POST\n  probed: true\n  unauthenticated_response: '{\"errors\":[{\"message\":\"You are not authorized\",\"extensions\":{\"code\":\"UNAUTHORIZED\"}}]}'\n  note: Live,\
  \ token-gated GraphQL endpoint confirmed on 2026-07-12.\ndomains:\n- domain: swapcard.com\n  dnssec: false\n  caa:\n  - '0 issue \"pki.goog\"'\n  - '0 issue \"amazonaws.com\"'\n  - '0 issue \"certainly.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issuewild \"amazonaws.com\"'\n  - '0 issuewild \"digicert.com\"'\n  - '0 issuewild \"letsencrypt.org\"'\n  - '0 issuewild \"pki.goog\"'\n  - '0 iodef \"mailto:security@swapcard.com\"'\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:_spf1.swapcard.com include:mail.zendesk.com include:3004554.spf03.hubspotemail.net include:app.outreach.io -all'\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swapcard/refs/heads/main/security/swapcard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Management
- Community
- Networking
- Event Platform
- GraphQL
- Attendees
- Exhibitors
- SaaS
---
