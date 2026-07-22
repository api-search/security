---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: subtlemedical.com
  spf: true
hosts:
- cert_expires: Mar 21 12:48:46 2027 GMT
  host: www.subtlemedical.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Subtle Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subtle Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Subtle Medical
provider_slug: subtle-medical
slug: subtle-medical-domain-security
source_filename: subtle-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subtlemedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 12:48:46 2027 GMT\n  hsts: null\ndomains:\n- domain: subtlemedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subtle-medical/refs/heads/main/security/subtle-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Deep Learning
- Radiology
- DICOM
- Diagnostics
---
