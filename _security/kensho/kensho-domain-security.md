---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kensho.com
  spf: true
hosts:
- cert_expires: Oct 12 13:45:18 2026 GMT
  host: kensho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: docs.kensho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: scribe.kensho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kensho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kensho, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kensho
provider_slug: kensho
slug: kensho-domain-security
source_filename: kensho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kensho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 13:45:18 2026 GMT\n  hsts: null\n- host: docs.kensho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\n- host: scribe.kensho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kensho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kensho/refs/heads/main/security/kensho-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Financial Data
- Speech to Text
- Transcription
- Document Extraction
- Named Entity Recognition
- Natural Language Processing
- LLM
- Model Context Protocol
- Retrieval
- S&P Global
---
