---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: labelbox.com
  spf: true
hosts:
- cert_expires: Sep 22 22:03:15 2026 GMT
  host: labelbox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 17:48:27 2026 GMT
  host: docs.labelbox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 00:43:12 2026 GMT
  host: api.labelbox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labelbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labelbox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Labelbox
provider_slug: labelbox
slug: labelbox-domain-security
source_filename: labelbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: labelbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.labelbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 17:48:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.labelbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:43:12 2026 GMT\n  hsts: null\ndomains:\n- domain: labelbox.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labelbox/refs/heads/main/security/labelbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Labeling
- AI Training
- Machine Learning
- Annotation
- Computer Vision
- RLHF
- Model Evaluation
- Dataset Management
- GraphQL
- Python SDK
---
