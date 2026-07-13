---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: MonkeyLearn API
  slug: monkeylearn-api
  spec_type: OpenAPI
  url: https://new.monkeylearn.com/api/v3/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: monkeylearn.com
  spf: true
hosts:
- cert_expires: Sep 14 12:27:43 2026 GMT
  host: monkeylearn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.monkeylearn.com
  https: false
kind: domain-security
layout: security
method: probed
name: Monkeylearn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MonkeyLearn, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MonkeyLearn
provider_slug: monkeylearn
slug: monkeylearn-domain-security
source_filename: monkeylearn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monkeylearn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:27:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.monkeylearn.com\n  https: false\ndomains:\n- domain: monkeylearn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monkeylearn/refs/heads/main/security/monkeylearn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text Analysis
- Machine Learning
- Sentiment Analysis
- Natural Language Processing
- Text Classification
- Keyword Extraction
- Artificial Intelligence
---
