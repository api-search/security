---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: el.ai
  spf: true
hosts:
- cert_expires: Oct 16 17:15:39 2026 GMT
  host: el.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Echo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echo Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Echo Labs
provider_slug: echo-labs
slug: echo-labs-domain-security
source_filename: echo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: el.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:15:39 2026 GMT\n  hsts: false\ndomains:\n- domain: el.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo-labs/refs/heads/main/security/echo-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Accessibility
- Captioning
- Audio Description
- Higher Education
- Video
- WCAG
- ADA Compliance
- Artificial Intelligence
---
