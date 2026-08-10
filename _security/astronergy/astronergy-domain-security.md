---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astronergy.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.astronergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astronergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astronergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Astronergy
provider_slug: astronergy
slug: astronergy-domain-security
source_filename: astronergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astronergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: astronergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronergy/refs/heads/main/security/astronergy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Solar
- Photovoltaic
- Renewable Energy
- Energy
- Manufacturing
- Hardware
- Sustainability
- Climate
---
