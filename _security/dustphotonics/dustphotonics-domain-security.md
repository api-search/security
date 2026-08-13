---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dustphotonics.com
  spf: true
hosts:
- cert_expires: Oct 21 18:38:19 2026 GMT
  host: www.dustphotonics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dustphotonics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DustPhotonics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DustPhotonics
provider_slug: dustphotonics
slug: dustphotonics-domain-security
source_filename: dustphotonics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dustphotonics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:38:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dustphotonics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dustphotonics/refs/heads/main/security/dustphotonics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Silicon Photonics
- Semiconductors
- Optical Interconnect
- Photonic Integrated Circuits
- Data Center Infrastructure
- AI Infrastructure
- Optical Transceivers
- Hardware
---
