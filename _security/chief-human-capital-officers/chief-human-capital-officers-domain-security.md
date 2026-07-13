---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: opm.gov
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.opm.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chief Human Capital Officers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chief Human Capital Officers Council, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chief Human Capital Officers Council
provider_slug: chief-human-capital-officers
slug: chief-human-capital-officers-domain-security
source_filename: chief-human-capital-officers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opm.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opm.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chief-human-capital-officers/refs/heads/main/security/chief-human-capital-officers-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- CHCO
- Federal Government
- HR Policy
- Human Capital
- Human Resources
- Interagency Council
- OPM
- Public Sector
- Talent Acquisition
- Workforce Management
---
