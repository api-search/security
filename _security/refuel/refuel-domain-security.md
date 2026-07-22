---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: refuel.ai
  spf: true
hosts:
- cert_expires: Sep 26 08:29:16 2026 GMT
  host: docs.refuel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 09:45:51 2026 GMT
  host: app.refuel.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refuel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refuel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Refuel
provider_slug: refuel
slug: refuel-domain-security
source_filename: refuel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.refuel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.refuel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 09:45:51 2026 GMT\n  hsts: null\ndomains:\n- domain: refuel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refuel/refs/heads/main/security/refuel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Labeling
- Machine Learning
- LLM
- Data Enrichment
- Artificial Intelligence
- Data Transformation
- MLOps
- SDK
---
