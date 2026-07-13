---
api_specs:
- filename: docs
  format: yaml
  label: Argilla REST API
  slug: argilla-rest-api
  spec_type: OpenAPI
  url: https://argilla.io/api/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: argilla.io
  spf: true
hosts:
- cert_expires: Aug 28 17:23:51 2026 GMT
  host: argilla.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:53:48 2026 GMT
  host: docs.argilla.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argilla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Argilla
provider_slug: argilla
slug: argilla-domain-security
source_filename: argilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.argilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:53:48 2026 GMT\n  hsts: false\ndomains:\n- domain: argilla.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/security/argilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- data annotation
- LLM
- NLP
- RLHF
- machine learning
- datasets
- open source
- human feedback
- fine-tuning
- Hugging Face
---
