---
api_specs:
- filename: reference
  format: yaml
  label: Rybbon Instant Rewards API
  slug: rybbon-instant-rewards-api
  spec_type: OpenAPI
  url: https://demo.rybbon.net/public/v2/reference
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bhnrewards.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rybbon.net
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.bhnrewards.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developer.bhnrewards.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.rybbon.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rybbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rybbon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rybbon
provider_slug: rybbon
slug: rybbon-domain-security
source_filename: rybbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bhnrewards.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bhnrewards.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.rybbon.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bhnrewards.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rybbon.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbon/refs/heads/main/security/rybbon-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Digital Rewards
- Gift Cards
- Prepaid Cards
- Incentives
- Marketing
- Employee Recognition
- Market Research
- Points
- FinTech
---
