---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mightybuildings.com
  spf: true
hosts:
- cert_expires: Sep 28 14:46:38 2026 GMT
  host: www.mightybuildings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mighty Buildings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mighty Buildings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mighty Buildings
provider_slug: mighty-buildings
slug: mighty-buildings-domain-security
source_filename: mighty-buildings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mightybuildings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:46:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mightybuildings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mighty-buildings/refs/heads/main/security/mighty-buildings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Technology
- Contech
- 3D Printing
- Additive Manufacturing
- Advanced Manufacturing
- Prefabrication
- Modular Housing
- Housing
- Real Estate
- Building Materials
- Robotics
- Sustainability
- Acquired
---
