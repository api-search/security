---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: solarenspace.com
  spf: true
hosts:
- cert_expires: Oct  1 08:33:18 2026 GMT
  host: www.solarenspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solaren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solaren, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Solaren
provider_slug: solaren
slug: solaren-domain-security
source_filename: solaren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solarenspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:33:18 2026 GMT\n  hsts: false\ndomains:\n- domain: solarenspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaren/refs/heads/main/security/solaren-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Electricity
- Renewable Energy
- Space
- Aerospace
- Satellites
- Solar Power
- Utilities
---
