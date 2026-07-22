---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: constellationenergy.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: constellation.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.constellationenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.constellation.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Constellation Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constellation Energy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Constellation Energy
provider_slug: constellation-energy
slug: constellation-energy-domain-security
source_filename: constellation-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.constellationenergy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: www.constellation.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: constellationenergy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: constellation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-energy/refs/heads/main/security/constellation-energy-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Clean Energy
- Electricity
- Energy
- Fortune 500
- Hydro
- Natural Gas
- Nuclear
- Solar
- Utility
- Wind
---
