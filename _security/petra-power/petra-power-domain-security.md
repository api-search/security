---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: petrapower.com
  spf: true
hosts:
- cert_expires: Aug 31 07:25:03 2026 GMT
  host: petrapower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petra Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Petra Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Petra Power
provider_slug: petra-power
slug: petra-power-domain-security
source_filename: petra-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: petrapower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:25:03 2026 GMT\n  hsts: false\ndomains:\n- domain: petrapower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petra-power/refs/heads/main/security/petra-power-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Power Generation
- Fuel Cells
- On-Site Power
- Backup Power
- Data Centers
- Clean Energy
---
