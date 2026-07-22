---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: miri.ai
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: miri.health
  spf: true
hosts:
- cert_expires: Aug 31 03:34:06 2026 GMT
  host: www.miri.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: miri.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.miri.health
  https: false
kind: domain-security
layout: security
method: probed
name: Miri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miri, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Miri
provider_slug: miri
slug: miri-domain-security
source_filename: miri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.miri.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:34:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: miri.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.miri.health\n  https: false\ndomains:\n- domain: miri.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: miri.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miri/refs/heads/main/security/miri-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Wellness
- Digital Health
- Telehealth
- Artificial Intelligence
- Patient Engagement
- Weight Loss
- SDK
- Webhooks
---
