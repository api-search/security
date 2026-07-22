---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digitalbridge.com
  spf: true
hosts:
- cert_expires: Sep  2 02:02:03 2026 GMT
  host: www.digitalbridge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colony Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colony Capital (DigitalBridge Group), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Colony Capital (DigitalBridge Group)
provider_slug: colony-capital
slug: colony-capital-domain-security
source_filename: colony-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalbridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: digitalbridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colony-capital/refs/heads/main/security/colony-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
- Digital Infrastructure
- Data Centers
- Cell Towers
- Fiber
- Edge Computing
- Alternative Asset Manager
- REIT
---
