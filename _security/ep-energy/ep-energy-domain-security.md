---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ep-energy.com
  spf: true
hosts:
- cert_expires: Jul 26 05:23:25 2026 GMT
  host: www.ep-energy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ep Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EP Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EP Energy
provider_slug: ep-energy
slug: ep-energy-domain-security
source_filename: ep-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ep-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 05:23:25 2026 GMT\n  hsts: false\ndomains:\n- domain: ep-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ep-energy/refs/heads/main/security/ep-energy-domain-security.yml
summary_line: TLSv1.3
tags:
- Energy
- Oil and Gas
- Defunct
- Bankruptcy
- Fortune 1000
---
