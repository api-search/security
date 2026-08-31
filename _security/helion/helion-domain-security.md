---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helionenergy.com
  spf: true
hosts:
- cert_expires: Aug 16 07:18:38 2026 GMT
  host: www.helionenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helion Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Helion Energy
provider_slug: helion
slug: helion-domain-security
source_filename: helion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helionenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:18:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helionenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helion/refs/heads/main/security/helion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fusion Energy
- Fusion Power
- Pulsed Fusion
- Field-Reversed Configuration
- FRC
- Magneto-Inertial Fusion
- Deuterium-Helium-3
- Aneutronic Fusion
- Direct Energy Conversion
- Polaris
- Orion
- Electricity Generation
- Clean Energy
- Microsoft PPA
- Nucor
- Hardware
---
