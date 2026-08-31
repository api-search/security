---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terawattinfrastructure.com
  spf: true
hosts:
- cert_expires: Oct  3 15:08:45 2026 GMT
  host: www.terawattinfrastructure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terawatt Infrastructure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terawatt Infrastructure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terawatt Infrastructure
provider_slug: terawatt-infrastructure
slug: terawatt-infrastructure-domain-security
source_filename: terawatt-infrastructure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terawattinfrastructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:08:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terawattinfrastructure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terawatt-infrastructure/refs/heads/main/security/terawatt-infrastructure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Fleet Management
- Transportation
- Logistics
- Infrastructure
- Sustainability
- Charging as a Service
---
