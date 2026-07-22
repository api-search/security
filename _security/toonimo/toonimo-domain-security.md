---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: toonimo.com
  mx: google-workspace
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:26161334.spf03.hubspotemail.net -all
hosts:
- host: www.toonimo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_version: '1.1'
  https: true
  tls_verified: true
kind: domain-security
layout: security
method: probed
name: Toonimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toonimo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Toonimo
provider_slug: toonimo
slug: toonimo-domain-security
source_filename: toonimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live probe of toonimo.com (curl TLS/HTTP HEAD + dig)\nhosts:\n  - host: www.toonimo.com\n    https: true\n    http_version: \"1.1\"\n    tls_verified: true\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: true\ndomains:\n  - domain: toonimo.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:_spf.google.com include:26161334.spf03.hubspotemail.net -all\"\n    dmarc: true\n    dmarc_policy: none\n    mx: google-workspace\nnotes: >-\n  HSTS is strong (max-age 31536000, includeSubDomains, preload). No DNSSEC and\n  no CAA records published. SPF present; DMARC published but policy is p=none\n  (monitor-only, not enforcing). Email handled by Google Workspace + HubSpot.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toonimo/refs/heads/main/security/toonimo-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- Digital Adoption
- Digital Adoption Platform
- Employee Onboarding
- User Onboarding
- Customer Success
- Guidance
- Self Service
- Enterprise Software
- Walkthroughs
---
