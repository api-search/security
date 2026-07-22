---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datasaur.ai
  spf: true
hosts:
- cert_expires: Aug 22 01:14:02 2026 GMT
  host: datasaur.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datasaur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datasaur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datasaur
provider_slug: datasaur
slug: datasaur-domain-security
source_filename: datasaur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datasaur.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 01:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datasaur.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datasaur/refs/heads/main/security/datasaur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Data Labeling
- Artificial Intelligence
- Machine Learning
- Large Language Models
- NLP
- Data Annotation
- GraphQL
---
