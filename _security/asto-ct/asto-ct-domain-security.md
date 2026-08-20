---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: astoct.com
  spf: true
hosts:
- cert_expires: Sep 22 23:54:16 2026 GMT
  host: www.astoct.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asto Ct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asto CT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Asto CT
provider_slug: asto-ct
slug: asto-ct-domain-security
source_filename: asto-ct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astoct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:54:16 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: astoct.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asto-ct/refs/heads/main/security/asto-ct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Medical Imaging
- Veterinary
- Equine Health
- Computed Tomography
- Healthcare
- Hardware
---
