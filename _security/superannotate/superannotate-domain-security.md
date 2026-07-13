---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: superannotate.com
  spf: true
hosts:
- cert_expires: Sep 28 08:14:20 2026 GMT
  host: www.superannotate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:31:22 2026 GMT
  host: doc.superannotate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.superannotate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superannotate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuperAnnotate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SuperAnnotate
provider_slug: superannotate
slug: superannotate-domain-security
source_filename: superannotate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superannotate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:14:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.superannotate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:31:22 2026 GMT\n  hsts: null\n- host: api.superannotate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: superannotate.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superannotate/refs/heads/main/security/superannotate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Annotation
- Data Labeling
- Computer Vision
- NLP
- Machine Learning
- Training Data
- Image Annotation
- Video Annotation
- Text Annotation
- Audio Annotation
- MLOps
---
