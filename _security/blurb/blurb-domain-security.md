---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blurb.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rpiprint.com
  spf: true
hosts:
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: www.blurb.com
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.rpiprint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blurb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blurb, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blurb
provider_slug: blurb
slug: blurb-domain-security
source_filename: blurb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blurb.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 600\n- host: api.rpiprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: blurb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rpiprint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blurb/refs/heads/main/security/blurb-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Publishing
- Printing
- Print on Demand
- Books
- Self Publishing
- Photo Books
- Fulfillment
- E-commerce
- API
---
