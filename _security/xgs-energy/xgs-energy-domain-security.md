---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xgsenergy.com
  spf: true
hosts:
- cert_expires: Oct 17 21:46:46 2026 GMT
  host: www.xgsenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xgs Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XGS Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: XGS Energy
provider_slug: xgs-energy
slug: xgs-energy-domain-security
source_filename: xgs-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xgsenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:46:46 2026 GMT\n  hsts: false\ndomains:\n- domain: xgsenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/security/xgs-energy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Geothermal
- Renewable Energy
- Clean Energy
- Power Generation
- Energy Infrastructure
- Data Center Power
- Climate Tech
---
