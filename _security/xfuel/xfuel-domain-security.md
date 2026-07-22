---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xfuel.com
  spf: true
hosts:
- cert_expires: Aug 31 14:49:50 2026 GMT
  host: xfuel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xfuel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XFuel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: XFuel
provider_slug: xfuel
slug: xfuel-domain-security
source_filename: xfuel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xfuel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:49:50 2026 GMT\n  hsts: false\ndomains:\n- domain: xfuel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xfuel/refs/heads/main/security/xfuel-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Biofuels
- Sustainability
- Transportation
- Climate
- Waste-to-Fuel
---
