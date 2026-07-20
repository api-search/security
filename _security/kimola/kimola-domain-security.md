---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kimola.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: kimola.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.kimola.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kimola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kimola, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kimola
provider_slug: kimola
slug: kimola-domain-security
source_filename: kimola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kimola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.kimola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kimola.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimola/refs/heads/main/security/kimola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Research
- Customer Feedback
- Text Analytics
- Sentiment Analysis
- Natural Language Processing
- Consumer Insights
- Machine Learning
- Artificial Intelligence
---
