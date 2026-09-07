---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adagiomedical.com
  spf: true
hosts:
- cert_expires: Nov 17 16:01:39 2026 GMT
  host: adagiomedical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adagiomedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adagio Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Adagio Medical
provider_slug: adagiomedical
slug: adagiomedical-domain-security
source_filename: adagiomedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adagiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 16:01:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adagiomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adagiomedical/refs/heads/main/security/adagiomedical-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Medical Devices
- Health
- Cardiology
- Medical Technology
- Cryoablation
- Electrophysiology
---
