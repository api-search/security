---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gardin.ag
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: gardin.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: developers.gardin.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.gardin.ag
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gardin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gardin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gardin
provider_slug: gardin
slug: gardin-domain-security
source_filename: gardin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gardin.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\n- host: developers.gardin.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\n- host: api.gardin.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gardin.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gardin/refs/heads/main/security/gardin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- Agritech
- Precision Agriculture
- Plant Health
- Photosynthesis
- IoT
- Sensors
- Greenhouse
- Crop Intelligence
- Sustainability
- Data
---
