---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kindor.co
  spf: false
hosts:
- cert_expires: Sep 14 14:19:48 2026 GMT
  host: kindor.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kindor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kindor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kindor
provider_slug: kindor
slug: kindor-domain-security
source_filename: kindor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kindor.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: kindor.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kindor/refs/heads/main/security/kindor-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Engineering Intelligence
- Developer Productivity
- DORA Metrics
- Software Delivery
- AI Adoption
- Analytics
- Reporting
---
