---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_subdomain_policy: none
  dnssec: false
  domain: greator.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:4472479.spf02.hubspotemail.net include:sendgrid.net include:mail.timmehosting.de ~all
hosts:
- cert_verify: ok
  host: greator.com
  hsts: false
  hsts_max_age: null
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Greator
provider_slug: greator
slug: greator-domain-security
source_filename: greator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: 'dig + TLS/HTTP HEAD probe of greator.com (apis.yml Website host)'\nhosts:\n  - host: greator.com\n    https: true\n    tls_version: TLSv1.3\n    cert_verify: ok\n    server: cloudflare\n    hsts: false\n    hsts_max_age: null\ndomains:\n  - domain: greator.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:_spf.google.com include:4472479.spf02.hubspotemail.net include:sendgrid.net include:mail.timmehosting.de ~all'\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_subdomain_policy: none\nnotes: >-\n  Website fronted by Cloudflare over TLS 1.3 with a valid certificate, but no\n  HSTS response header and no CAA records. Zone is not DNSSEC-signed. Email\n  authentication is configured: SPF present (Google/HubSpot/SendGrid senders)\n  and a DMARC record at p=quarantine (sp=none). Absence of CAA/HSTS/DNSSEC is\n  recorded as-observed, not inferred.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greator/refs/heads/main/security/greator-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Personal Development
- Coaching
- Online Learning
- E-Learning
- Wellness
- Events
- Germany
---
