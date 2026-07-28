---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joltcharge.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jolt.com.au
  note: Only Google site-verification TXT records are published on this domain; no SPF record was returned. DMARC is present but set to p=none (monitor only).
  spf: false
hosts:
- cert_expires: Sep 24 09:29:54 2026 GMT
  host: joltcharge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 04:02:56 2026 GMT
  host: api.joltcharge.com
  hsts: false
  https: true
  note: Cloudflare-fronted. The host root serves a static S3 app-deep-link page; the /v1/ prefix routes to an AWS API Gateway stage that answers 401 Unauthorized on every path and method probed anonymously.
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:16:39 2026 GMT
  host: jolt.com.au
  hsts: false
  https: true
  note: Legacy primary domain; 301-redirects to https://joltcharge.com/au/.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jolt Charge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JOLT, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JOLT
provider_slug: jolt-charge
slug: jolt-charge-domain-security
source_filename: jolt-charge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the api.joltcharge.com and\n  jolt.com.au hosts observed in the JOLT website bundle and redirect chain\nhosts:\n- host: joltcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:29:54 2026 GMT\n  hsts: false\n- host: api.joltcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:02:56 2026 GMT\n  hsts: false\n  note: Cloudflare-fronted. The host root serves a static S3 app-deep-link page; the\n    /v1/ prefix routes to an AWS API Gateway stage that answers 401 Unauthorized on\n    every path and method probed anonymously.\n- host: jolt.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:16:39 2026 GMT\n  hsts: false\n  note: Legacy primary domain; 301-redirects to https://joltcharge.com/au/.\ndomains:\n- domain: joltcharge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain:\
  \ jolt.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  note: Only Google site-verification TXT records are published on this domain; no\n    SPF record was returned. DMARC is present but set to p=none (monitor only).\nfindings:\n- No HSTS on any JOLT host probed.\n- No CAA records and no DNSSEC on either registrable domain.\n- Email authentication is stronger on joltcharge.com (SPF + DMARC quarantine) than\n  on the legacy jolt.com.au domain (no SPF, DMARC p=none).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jolt-charge/refs/heads/main/security/jolt-charge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Australia
- EV Charging
- Electricity
- Utilities
- Renewables
- Advertising
- Mobility
- Carbon
- Infrastructure
---
