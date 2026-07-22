---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pulselabs.ai
  spf: true
hosts:
- cert_expires: Sep  6 03:14:26 2026 GMT
  host: pulselabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulse Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pulse Labs
provider_slug: pulse-labs
slug: pulse-labs-domain-security
source_filename: pulse-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulselabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:14:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pulselabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-labs/refs/heads/main/security/pulse-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- User Research
- UX
- Product
- Surveys
- Feedback
- SDK
- Design
- Artificial Intelligence
---
