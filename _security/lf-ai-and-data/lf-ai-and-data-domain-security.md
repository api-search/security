---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lfaidata.foundation
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: onnx.ai
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: lfaidata.foundation
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:59:20 2026 GMT
  host: onnx.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: milvus.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lf Ai And Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LF AI and Data, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LF AI and Data
provider_slug: lf-ai-and-data
slug: lf-ai-and-data-domain-security
source_filename: lf-ai-and-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lfaidata.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: onnx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:59:20 2026 GMT\n  hsts: false\n- host: milvus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lfaidata.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: onnx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lf-ai-and-data/refs/heads/main/security/lf-ai-and-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Machine Learning
- Data
- Linux Foundation
- Open Source
- MLOps
- Vector Database
---
