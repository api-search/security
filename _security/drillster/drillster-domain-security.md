---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  caa_note: An earlier probe (2026-07-11) also recorded digicert.com and comodoca.com issue records; the current CAA set is narrower.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: drillster.com
  spf: true
hosts:
- cert_expires: Nov 28 19:37:15 2026 GMT
  host: www.drillster.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  role: API host, developer documentation, console, OAuth authorization server
  tls_version: TLSv1.3
- host: drillster.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: marketing site (separate Next.js application)
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Drillster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drillster, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Drillster
provider_slug: drillster
slug: drillster-domain-security
source_filename: drillster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of the hosts in apis.yml plus the API base host\n  (https://www.drillster.com/api/2.1.1). Baseline written by\n  0-working/probe-domain-security.py, then corrected by hand — see hsts_note.\nhosts:\n  - host: www.drillster.com\n    role: API host, developer documentation, console, OAuth authorization server\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Nov 28 19:37:15 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: true\n    hsts_header: 'max-age=31536000; includeSubDomains; preload'\n  - host: drillster.com\n    role: marketing site (separate Next.js application)\n    https: true\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: false\n    hsts_header: 'max-age=31536000; includeSubDomains'\nhsts_note: >-\n  The automated probe recorded hsts: null for www.drillster.com on this\
  \ run. That was a false\n  negative: a live HEAD of https://www.drillster.com/, of the developer documentation, and of\n  https://www.drillster.com/api/2.1.1/version each returned\n  strict-transport-security: max-age=31536000; includeSubDomains; preload on 2026-09-06.\n  Corrected here with the header quoted verbatim.\nresponse_security_headers:\n  observed_on: https://www.drillster.com/api/2.1.1/version\n  date: '2026-09-06'\n  headers:\n    x-content-type-options: nosniff\n    x-frame-options: DENY\n    referrer-policy: no-referrer\n    x-xss-protection: '0'\n    cache-control: no-cache, no-store, max-age=0, must-revalidate\ndomains:\n  - domain: drillster.com\n    dnssec: true\n    caa:\n      - 0 issue \"pki.goog\"\n      - 0 issue \"letsencrypt.org\"\n    spf: true\n    dmarc: true\n    dmarc_policy: quarantine\n    caa_note: >-\n      An earlier probe (2026-07-11) also recorded digicert.com and comodoca.com issue records;\n      the current CAA set is narrower.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillster/refs/heads/main/security/drillster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Assessments
- Education
- Learning
- Quizzes
- Training
- LMS
- Adaptive Learning
- Compliance Training
- Webhooks
---
