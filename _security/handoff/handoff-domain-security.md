---
description: ''
domains:
- caa:
  - dwyt1s0tpmwz.cloudfront.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: handoff.ai
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: handoff.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Handoff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handoff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Handoff
provider_slug: handoff
slug: handoff-domain-security
source_filename: handoff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handoff.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: handoff.ai\n  dnssec: true\n  caa:\n  - dwyt1s0tpmwz.cloudfront.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handoff/refs/heads/main/security/handoff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Construction
- Construction Management
- Estimating
- Takeoffs
- Contractors
- Artificial Intelligence
- Project Management
- CRM
- Field Service
---
