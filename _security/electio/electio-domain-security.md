---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: electiotechnologies.com
  spf: true
hosts:
- cert_expires: Oct  4 15:16:16 2026 GMT
  host: www.electiotechnologies.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Electio
provider_slug: electio
slug: electio-domain-security
source_filename: electio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.electiotechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:16:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: electiotechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electio/refs/heads/main/security/electio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Infrastructure
- Control Systems
- Industrial Software
- Transportation
- Automation
- Stealth
---
