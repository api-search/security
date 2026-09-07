---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bd.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.bd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carefusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareFusion (BD), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CareFusion (BD)
provider_slug: carefusion
slug: carefusion-domain-security
source_filename: carefusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carefusion/refs/heads/main/security/carefusion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automated Dispensing
- BD
- CareFusion
- Connected Devices
- EMR Integration
- Healthcare
- HL7
- Infusion Pumps
- Medical Devices
- Pyxis
- Smart Pumps
---
