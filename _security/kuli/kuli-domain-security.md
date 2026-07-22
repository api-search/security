---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kuli.one
  spf: true
hosts:
- cert_expires: Oct  2 10:03:46 2026 GMT
  host: kuli.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kuli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kuli
provider_slug: kuli
slug: kuli-domain-security
source_filename: kuli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kuli.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kuli.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuli/refs/heads/main/security/kuli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Influencer Marketing
- Marketing
- Artificial Intelligence
- Creator Economy
- Brand Safety
- Video Analysis
- Social Media
---
