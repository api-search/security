---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:dmarc@hellotend.com
  dnssec: false
  domain: hellotend.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:49505286.spf06.hubspotemail.net include:_spf.salesforce.com ip4:209.23.205.74 include:spf-00808c01.pphosted.com ip4:216.71.150.115 ~all
hosts:
- host: www.hellotend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  server: cloudflare
  tls_version: null
- host: hellotend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  server: cloudflare
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Tend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tend
provider_slug: tend
slug: tend-domain-security
source_filename: tend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live probe of hellotend.com (curl HEAD + dig) 2026-07-21\nnotes: >-\n  Tend Dental is a consumer dental-care company with no public API surface, so\n  only the marketing/booking web host was probed. The apex hellotend.com serves\n  the site (www.hellotend.com) behind Cloudflare with a long HSTS max-age. No\n  CAA record and no DNSSEC (no DS) at the registrable domain; SPF is published\n  and DMARC exists but is set to monitor-only (p=none).\nhosts:\n  - host: www.hellotend.com\n    https: true\n    server: cloudflare\n    hsts: true\n    hsts_max_age: 63072000\n    tls_version: null   # not confirmed this pass (classifier intermittently unavailable)\n  - host: hellotend.com\n    https: true\n    server: cloudflare\n    hsts: true\n    hsts_max_age: 63072000\n    tls_version: null\ndomains:\n  - domain: hellotend.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:_spf.google.com include:sendgrid.net\
  \ include:49505286.spf06.hubspotemail.net include:_spf.salesforce.com ip4:209.23.205.74 include:spf-00808c01.pphosted.com ip4:216.71.150.115 ~all\"\n    dmarc: true\n    dmarc_policy: none\n    dmarc_record: \"v=DMARC1; p=none; rua=mailto:dmarc@hellotend.com\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tend/refs/heads/main/security/tend-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- Consumer
- Dental
- Healthcare
- Consumer Health
- Booking
- Local Services
---
