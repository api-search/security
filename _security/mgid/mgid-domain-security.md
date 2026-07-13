---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mgid.com
  spf: true
hosts:
- cert_expires: Sep 13 10:46:43 2026 GMT
  host: www.mgid.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:50:11 2026 GMT
  host: help.mgid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 10:46:43 2026 GMT
  host: api.mgid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mgid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MGID, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MGID
provider_slug: mgid
slug: mgid-domain-security
source_filename: mgid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mgid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:46:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: help.mgid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:50:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mgid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:46:43 2026 GMT\n  hsts: null\ndomains:\n- domain: mgid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mgid/refs/heads/main/security/mgid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Native Advertising
- Ad Tech
- Publishers
- Advertisers
- Campaigns
- Content Monetization
- Programmatic
---
