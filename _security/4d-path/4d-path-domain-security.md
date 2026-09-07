---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 4dpath.com
  spf: true
hosts:
- cert_expires: Nov 28 15:23:41 2026 GMT
  host: 4dpath.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4D Path Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4D Path, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 4D Path
provider_slug: 4d-path
slug: 4d-path-domain-security
source_filename: 4d-path-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4dpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 15:23:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 4dpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4d-path/refs/heads/main/security/4d-path-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Digital Pathology
- Oncology
- Cancer Diagnostics
- Medical Imaging
- Artificial Intelligence
- Precision Medicine
- Software As A Medical Device
- Life Sciences
- Massachusetts
---
