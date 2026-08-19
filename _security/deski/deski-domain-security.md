---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@deski.ai"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heartfocus.ai
  spf: true
hosts:
- cert_expires: Sep 29 23:14:27 2026 GMT
  host: www.heartfocus.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deski Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DESKi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DESKi
provider_slug: deski
slug: deski-domain-security
source_filename: deski-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heartfocus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:14:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heartfocus.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@deski.ai\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deski/refs/heads/main/security/deski-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthtech
- Medical Imaging
- Cardiology
- Ultrasound
- Point-of-Care Ultrasound
- Artificial Intelligence
- Medical Device
- DICOM
- France
---
