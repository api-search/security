---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: circulargenomics.com
  spf: true
hosts:
- cert_expires: Oct  9 23:39:28 2026 GMT
  host: www.circulargenomics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: mindlight.circulargenomics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'Login-gated provider portal for test ordering and results delivery. Served by CrelioHealth (Creliant Software Pvt. Ltd.) — response carries `server: Crelio` and the page is a white-labeled CrelioHealth LIS, not a first-party Circular Genomics application.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circular Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circular Genomics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Circular Genomics
provider_slug: circular-genomics
slug: circular-genomics-domain-security
source_filename: circular-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.circulargenomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mindlight.circulargenomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    Login-gated provider portal for test ordering and results delivery. Served by\n    CrelioHealth (Creliant Software Pvt. Ltd.) — response carries `server: Crelio`\n    and the page is a white-labeled CrelioHealth LIS, not a first-party Circular\n    Genomics application.\ndomains:\n- domain: circulargenomics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circular-genomics/refs/heads/main/security/circular-genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Diagnostics
- Genomics
- Precision Medicine
- Neurology
- Life Sciences
- Health
- Clinical Laboratory
- Biomarkers
---
