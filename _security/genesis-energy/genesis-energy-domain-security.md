---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genesis-energy.com
  spf: false
hosts:
- cert_expires: Dec 26 06:18:15 2026 GMT
  host: www.genesis-energy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genesis Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Genesis Energy
provider_slug: genesis-energy
slug: genesis-energy-domain-security
source_filename: genesis-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genesis-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 06:18:15 2026 GMT\n  hsts: false\ndomains:\n- domain: genesis-energy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesis-energy/refs/heads/main/security/genesis-energy-domain-security.yml
summary_line: TLSv1.3
tags:
- Energy
- Midstream
- Oil and Gas
---
