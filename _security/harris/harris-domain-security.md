---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harriscomputer.com
  spf: true
hosts:
- cert_expires: Aug 30 09:01:58 2026 GMT
  host: www.harriscomputer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harris Computer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harris Computer
provider_slug: harris
slug: harris-domain-security
source_filename: harris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harriscomputer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 09:01:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: harriscomputer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harris/refs/heads/main/security/harris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Financial Services
- Healthcare
- Insurance
- Public Sector
- Utilities
- Vertical Market Software
- Fortune 500
---
