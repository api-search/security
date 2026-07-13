---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: encord.com
  spf: true
hosts:
- cert_expires: Aug 27 13:41:02 2026 GMT
  host: encord.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 14:55:14 2026 GMT
  host: docs.encord.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 13:50:26 2026 GMT
  host: api.encord.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Encord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encord, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Encord
provider_slug: encord
slug: encord-domain-security
source_filename: encord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: encord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:41:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: docs.encord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:55:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.encord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:50:26 2026 GMT\n  hsts: null\ndomains:\n- domain: encord.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encord/refs/heads/main/security/encord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Computer Vision
- Data Labeling
- Annotation
- Machine Learning
- Model Evaluation
- Dataset Management
- Artificial Intelligence
- Image Annotation
- Video Annotation
- DICOM
- Active Learning
- Quality Assurance
---
