---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kadeya.com
  spf: true
hosts:
- cert_expires: Sep 25 18:08:17 2026 GMT
  host: kadeya.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kadeya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadeya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kadeya
provider_slug: kadeya
slug: kadeya-domain-security
source_filename: kadeya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kadeya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:08:17 2026 GMT\n  hsts: null\ndomains:\n- domain: kadeya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadeya/refs/heads/main/security/kadeya-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate Technology
- Sustainability
- Beverage
- Hydration
- Reusable Packaging
- Vending
- Circular Economy
- Workplace
---
