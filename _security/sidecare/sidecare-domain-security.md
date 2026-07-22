---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sidecare.com
  spf: true
hosts:
- cert_expires: Sep  7 16:56:29 2026 GMT
  host: www.sidecare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidecare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SideCare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SideCare
provider_slug: sidecare
slug: sidecare-domain-security
source_filename: sidecare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sidecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 16:56:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sidecare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidecare/refs/heads/main/security/sidecare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Insurance
- Insurtech
- Health Insurance
- Employee Benefits
- Human Resources
- HRIS
- France
- OpenID Connect
---
