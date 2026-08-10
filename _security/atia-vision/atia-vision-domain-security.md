---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atiavision.com
  spf: true
hosts:
- cert_expires: Oct  1 04:10:52 2026 GMT
  host: atiavision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atia Vision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atia Vision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Atia Vision
provider_slug: atia-vision
slug: atia-vision-domain-security
source_filename: atia-vision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atiavision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:10:52 2026 GMT\n  hsts: false\ndomains:\n- domain: atiavision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atia-vision/refs/heads/main/security/atia-vision-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Medical Devices
- Ophthalmology
- Intraocular Lens
- Cataract Surgery
- Health
- Clinical Stage
---
