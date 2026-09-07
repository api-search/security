---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heartrecovery.com
  spf: true
hosts:
- cert_expires: Nov 26 16:06:36 2026 GMT
  host: www.heartrecovery.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abiomed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abiomed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abiomed
provider_slug: abiomed
slug: abiomed-domain-security
source_filename: abiomed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heartrecovery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heartrecovery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abiomed/refs/heads/main/security/abiomed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Cardiology
- Mechanical Circulatory Support
- Heart Pumps
- Medical Technology
- Hospitals
- Clinical Support
- Life Sciences
---
