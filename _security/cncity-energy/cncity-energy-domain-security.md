---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cncityenergy.com
  spf: false
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.cncityenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cncity Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CNCITY Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CNCITY Energy
provider_slug: cncity-energy
slug: cncity-energy-domain-security
source_filename: cncity-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cncityenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cncityenergy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cncity-energy/refs/heads/main/security/cncity-energy-domain-security.yml
summary_line: TLSv1.3
tags:
- Energy
- Utilities
- Gas
- Electricity
- DistrictHeating
- South Korea
---
