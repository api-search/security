---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oklo.com
  spf: true
hosts:
- cert_expires: Aug 11 20:48:38 2026 GMT
  host: oklo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oklo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oklo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oklo
provider_slug: oklo
slug: oklo-domain-security
source_filename: oklo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oklo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 20:48:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oklo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oklo/refs/heads/main/security/oklo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Nuclear
- Advanced Fission
- Small Modular Reactor
- Fast Reactor
- Sodium Cooled
- HALEU
- Aurora Powerhouse
- Fuel Recycling
- Radioisotopes
- Clean Energy
- Data Center Power
- Hardware
---
