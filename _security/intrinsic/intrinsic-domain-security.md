---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withintrinsic.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: intrinsicapi.com
  spf: false
hosts:
- cert_expires: Aug 31 19:24:36 2026 GMT
  host: withintrinsic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 12:04:46 2026 GMT
  host: docs.intrinsicapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:35:30 2026 GMT
  host: api.intrinsicapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Intrinsic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intrinsic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Intrinsic
provider_slug: intrinsic
slug: intrinsic-domain-security
source_filename: intrinsic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withintrinsic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:24:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.intrinsicapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:04:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.intrinsicapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 10:35:30 2026 GMT\n  hsts: null\ndomains:\n- domain: withintrinsic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: intrinsicapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intrinsic/refs/heads/main/security/intrinsic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trust and Safety
- Content Moderation
- Anti-Abuse
- Fraud Detection
- Machine Learning
- Risk Intelligence
- API
---
