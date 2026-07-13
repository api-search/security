---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: siemens-healthineers.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: siemens.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.siemens-healthineers.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: marketplace.teamplay.siemens.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siemens Healthineers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siemens Healthineers, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Siemens Healthineers
provider_slug: siemens-healthineers
slug: siemens-healthineers-domain-security
source_filename: siemens-healthineers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siemens-healthineers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: marketplace.teamplay.siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: siemens-healthineers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: siemens.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens-healthineers/refs/heads/main/security/siemens-healthineers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Medical Imaging
- Laboratory Diagnostics
- Cancer Care
- Radiation Oncology
- DICOM
- Digital Health
- Healthcare IT
- Medical Devices
- Teamplay
---
