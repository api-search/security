---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: verra.org
  spf: true
hosts:
- cert_expires: Sep  1 05:23:34 2026 GMT
  host: verra.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verra Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Verra
provider_slug: verra-org
slug: verra-org-domain-security
source_filename: verra-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 05:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: verra.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verra-org/refs/heads/main/security/verra-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon
- Carbon Credits
- Carbon Markets
- Voluntary Carbon Market
- Carbon Registry
- Climate
- Climate Action
- Greenhouse Gas
- Emissions Reduction
- Offsets
- Sustainability
- Sustainable Development
- REDD+
- Forestry
- AFOLU
- Nature-Based Solutions
- Plastic Waste
- Standards
- Certification
- Nonprofit
---
