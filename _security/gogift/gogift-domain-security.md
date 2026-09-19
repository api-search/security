---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gogift.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gogift.io
  spf: true
hosts:
- cert_expires: Nov 14 20:00:18 2026 GMT
  host: global.gogift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 12:22:49 2026 GMT
  host: docs.gogift.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.gogift.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Gogift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoGift, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoGift
provider_slug: gogift
slug: gogift-domain-security
source_filename: gogift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.gogift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 20:00:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gogift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 12:22:49 2026 GMT\n  hsts: false\n- host: api.gogift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gogift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gogift.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gogift/refs/heads/main/security/gogift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gift Cards
- Rewards
- Incentives
- Loyalty
- Commerce
- Payments
- Employee Recognition
---
