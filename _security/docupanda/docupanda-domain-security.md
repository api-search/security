---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docupipe.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docupanda.io
  spf: true
hosts:
- cert_expires: Aug 13 01:14:53 2026 GMT
  host: www.docupipe.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:56:05 2026 GMT
  host: www.docupanda.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:15:40 2026 GMT
  host: docs.docupipe.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docupanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocuPanda, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DocuPanda
provider_slug: docupanda
slug: docupanda-domain-security
source_filename: docupanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docupipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:14:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.docupanda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:56:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.docupipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:15:40 2026 GMT\n  hsts: null\ndomains:\n- domain: docupipe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: docupanda.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/security/docupanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Document Extraction
- Document Intelligence
- IDP
- OCR
- Document AI
---
